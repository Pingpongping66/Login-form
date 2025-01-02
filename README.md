<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #fff;
    }

    .container {
      position: relative;
      width: 90%;
      max-width: 400px;
    }

    .background-shapes {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -1;
      overflow: hidden;
    }

    .shape {
      position: absolute;
      border-radius: 20px;
      opacity: 0.9;
    }

    .shape1 {
      background-color: #fdbd68;
      width: 200px;
      height: 200px;
      top: -50px;
      left: -50px;
      transform: rotate(45deg);
    }

    .shape2 {
      background-color: #a58ae4;
      width: 300px;
      height: 300px;
      bottom: -100px;
      right: -50px;
      transform: rotate(-30deg);
    }

    .login-form {
      background-color: #fdbd68;
      border-radius: 20px;
      padding: 20px;
      text-align: center;
    }

    .login-form h1 {
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 20px;
      color: #000;
      text-decoration: underline;
    }

    .input-group {
      margin-bottom: 15px;
      text-align: left;
    }

    .input-group label {
      font-size: 1rem;
      color: #000;
      margin-bottom: 5px;
      display: block;
    }

    .input-group input {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1rem;
    }

    .forgot-password {
      font-size: 0.9rem;
      color: #a58ae4;
      text-decoration: none;
      display: block;
      margin: 10px 0;
    }

    .login-btn {
      width: 100%;
      padding: 10px;
      background-color: #a58ae4;
      color: #fff;
      font-size: 1.2rem;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .login-btn:hover {
      background-color: #7f68d0;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="background-shapes">
      <div class="shape shape1"></div>
      <div class="shape shape2"></div>
    </div>
    <div class="login-form">
      <h1>Login</h1>
      <form>
        <div class="input-group">
          <label for="username">Username</label>
          <input type="text" id="username" placeholder="Enter your username">
        </div>
        <div class="input-group">
          <label for="password">Password</label>
          <input type="password" id="password" placeholder="Enter your password">
        </div>
        <a href="#" class="forgot-password">Forgot password?</a>
        <button type="submit" class="login-btn">Login</button>
      </form>
    </div>
  </div>
</body>
</html>
