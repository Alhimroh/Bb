<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
    form {
      border: 1px solid #ccc;
      padding: 20px;
      border-radius: 8px;
      width: 300px;
    }
    label {
      display: block;
      margin-bottom: 8px;
    }
    input {
      width: 100%;
      padding: 8px;
      margin-bottom: 12px;
      box-sizing: border-box;
    }
    button {
      background-color: #4CAF50;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <form id="loginForm">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>

    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <button type="button" onclick="login()">Login</button>
  </form>

  <script>
    function login() {
      var username = document.getElementById("username").value;
      var password = document.getElementById("password").value;

      // Mock authentication, replace with actual logic
      if (username === "user" && password === "pass") {
        alert("Login successful!");
      } else {
        alert("Login failed. Please check your credentials.");
      }
    }
  </script>

</body>
</html>
