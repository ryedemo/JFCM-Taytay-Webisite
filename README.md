<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background: url('https://source.unsplash.com/featured/?church') no-repeat center center/cover;
      position: relative;
    }
    body::before {
      content: "";
      position: absolute; top:0; left:0; right:0; bottom:0;
      background: rgba(0, 0, 0, 0.5);
    }
    .login-box {
      position: relative;
      background: rgba(255, 255, 255, 0.95);
      padding: 30px 25px;
      border-radius: 15px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.3);
      width: 320px;
      text-align: center;
      animation: fadeIn 1s ease-in-out;
    }
    .login-box img {
      width: 120px;
      border-radius: 50%;
      margin-bottom: 15px;
    }
    input {
      width: 90%;
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
      outline: none;
      transition: 0.3s;
    }
    input:focus {
      border-color: #4285F4;
      box-shadow: 0 0 8px rgba(66, 133, 244, 0.5);
    }
    button {
      background: #4285F4;
      color: white;
      border: none;
      padding: 12px;
      border-radius: 8px;
      cursor: pointer;
      width: 100%;
    }
    button:hover {
      background: #357ae8;
    }
    .error {
      color: red;
      margin-top: 12px;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.9); }
      to { opacity: 1; transform: scale(1); }
    }
  </style>
</head>
<body>
  <div class="login-box">
    <!-- Your church photo -->
    <img src="https://scontent.fmnl17-4.fna.fbcdn.net/v/t39.30808-6/476758085_1025079269656180_1508840151996929921_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=cc71e4&_nc_ohc=_ReU3GkJs5AQ7kNvwFJtgKv&_nc_oc=AdlPpscxYoBe9g4Dae6SXd8SP9S1_ioA207PYbYorCAA2QByrjCRxwWvleUdvUgoz7A&_nc_zt=23&_nc_ht=scontent.fmnl17-4.fna&_nc_gid=rNGOeXVRL6gYiNrY_w5yVw&oh=00_AfWz7u00hw-Q-ujEWO02yQqilGzzQA6cCDw7sTmJ5hjTrQ&oe=68BAFD37" 
         alt="Church Logo">

    <h2>Jesus First Christian Ministries-Taytay</h2>
    <input type="text" id="username" placeholder="Enter Username">
    <input type="password" id="password" placeholder="Enter Password">
    <button onclick="login()">Login</button>
    <p class="error" id="error-message"></p>
  </div>

  <script>
    function login() {
      const defaultUser = "admin";
      const defaultPass = "12345";
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;

      if (username === defaultUser && password === defaultPass) {
        window.location.href = "[https://drive.google.com/drive/my-drive](https://drive.google.com/drive/folders/1i2AuG5zaVImN4wnDyzYrqPGLH-B3iqCP?usp=sharing)";
      } else {
        document.getElementById("error-message").textContent = "Invalid username or password!";
      }
    }
  </script>
</body>
</html>
