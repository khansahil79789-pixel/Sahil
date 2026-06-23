<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ludo Tournament Demo</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Ludo Tournament</h1>
</header>

<nav>
    <button onclick="showPage('home')">Home</button>
    <button onclick="showPage('profile')">Profile</button>
    <button onclick="showPage('tournament')">Tournament</button>
    <button onclick="showPage('admin')">Admin</button>
</nav>

<section id="home" class="page">
    <h2>Welcome</h2>
    <p>Play Demo Ludo Tournaments</p>
</section>

<section id="profile" class="page hidden">
    <h2>User Profile</h2>
    <input type="text" placeholder="Username">
    <button>Update</button>
</section>

<section id="tournament" class="page hidden">
    <h2>Create Match</h2>
    <input type="text" id="matchName" placeholder="Match Name">
    <button onclick="createMatch()">Create Match</button>

    <h3>Available Matches</h3>
    <ul id="matchList"></ul>
</section>

<section id="admin" class="page hidden">
    <h2>Admin Dashboard</h2>
    <div class="card">
        <h3>Total Users</h3>
        <p>100</p>
    </div>

    <div class="card">
        <h3>Total Matches</h3>
        <p id="totalMatches">0</p>
    </div>
</section>

<script src="script.js"></script>
</body>
</html>
