---
trigger: glob
glob: *.php,*.html,*.js,*.sql
---
Vanilla Web Standards - PHP/HTML/JS/SQLite/MariaDB
Principles
PHP pure (no Laravel/Symfony). Custom, lightweight.

No frameworks. PDO for DB, prepared statements only.

JS vanilla (no React/Vue). Min allocs, efficient DOM.

DB: Indexes everywhere, JOINs optimized, no SELECT *.

Security/Perf
Sanitize ALL inputs (filter_var, htmlspecialchars).

Sessions secure, CSRF tokens.

Cache queries, connection pooling.

Example PHP
php
<?php
$pdo = new PDO('mysql:host=localhost;dbname=test', $user, $pass);
$stmt = $pdo->prepare('SELECT * FROM users WHERE id = ?');
$stmt->execute([$_GET['id'] ?? 0]);
$user = $stmt->fetch(PDO::FETCH_ASSOC);
?>