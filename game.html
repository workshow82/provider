<?php

$conn = new mysqli("localhost","u544098814_allapi","Developer@987654","u544098814_allapi");
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}

// Get game_api name from URL
$gameApi = isset($_GET['name']) ? trim($_GET['name']) : '';

if (empty($gameApi)) {
    echo "No game provider selected.";
    exit;
}

// Fetch game data
$stmt = $conn->prepare("SELECT game_id, game_name FROM api_data WHERE game_api = ?");
$stmt->bind_param("s", $gameApi);
$stmt->execute();
$result = $stmt->get_result();
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Games by <?= htmlspecialchars($gameApi) ?></title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">
<div class="container py-4">
    <h2 class="mb-4">Games from: <?= htmlspecialchars($gameApi) ?></h2>

    <div class="row row-cols-1 row-cols-md-3 g-4">
        <?php if ($result->num_rows > 0): ?>
            <?php while ($row = $result->fetch_assoc()): ?>
                <div class="col">
                    <div class="card h-100 shadow-sm text-center">
                        <div class="card-body">
                            <h5 class="card-title"><?= htmlspecialchars($row['game_name']) ?></h5>
                            <a href="../sonu1.php?gameid=<?= urlencode($row['game_id']) ?>"
                               class="btn btn-primary mt-3">
                                🎮 Launch Game
                            </a>
                        </div>
                    </div>
                </div>
            <?php endwhile; ?>
        <?php else: ?>
            <p>No games found for this provider.</p>
        <?php endif; ?>
    </div>
</div>
</body>
</html>

<?php
$stmt->close();
$conn->close();
?>
