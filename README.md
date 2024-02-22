<form id="loginForm">
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="password">Password:</label><br>
  <input type="password" id="password" name="password"><br>
  <input type="submit" value="Login">
</form>
body {
  font-family: Arial, sans-serif;
}

form {
  width: 300px;
  margin: 0 auto;
}

input[type="text"], input[type="password"] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

input[type="submit"] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  display: inline-block;
}document.querySelector('#loginForm').addEventListener('submit', function(e) {
  var username = document.querySelector('#username').value;
  var password = document.querySelector('#password').value;
  
  if (!username || !password) {
    alert('Masukkan username dan password!');
    e.preventDefault();
  }
});if (username && password) {
  localStorage.setItem('username', username);
  localStorage.setItem('password', password);
}
