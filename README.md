<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Team Burton</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: #ffffff;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        nav {
            background-color: #333;
            overflow: hidden;
        }
        nav a {
            float: left;
            display: block;
            color: #f2f2f2;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #ddd;
            color: black;
        }
        header {
            background-color: #1f1f1f;
            padding: 20px;
        }
        header h1 {
            margin: 0;
        }
        section {
            padding: 20px;
        }
        footer {
            background-color: #1f1f1f;
            padding: 10px;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
<header>
    <h1>Team Burton</h1>
</header>
<div id="nav-placeholder"></div>
<script>
    fetch('/pages/nav.html')
        .then(response => response.text())
        .then(data => {
            document.getElementById('nav-placeholder').innerHTML = data;
        });
</script>
<section>
    <h2>Welcome to Team Burton's Official Website</h2>
    <p>We are a CTF's group</p>
    <p>Our motto: "Shadows whisper what light can not reveal."</p>
    <footer>
    <p>&copy; 2025 Team Burton. All rights reserved.</p>
    </footer>
</section>
</body>
</html>
