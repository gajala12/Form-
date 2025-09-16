<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Register</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f5f6fa;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .container {
      display: flex;
      width: 900px;
      max-width: 100%;
      background: #fff;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      flex-direction: row;
    }

    .form-box {
      flex: 1;
      padding: 40px;
    }

    .form-box h2 {
      font-size: 28px;
      margin-bottom: 10px;
      color: #222;
    }

    .form-box p {
      color: #888;
      margin-bottom: 30px;
      font-size: 14px;
    }

    .form-group {
      display: flex;
      gap: 20px;
      margin-bottom: 20px;
      flex-wrap: wrap;
    }

    .form-group input {
      flex: 1;
      min-width: 100px;
      padding: 12px 15px;
      border: 1px solid #ddd;
      border-radius: 5px;
      font-size: 14px;
      outline: none;
      transition: border 0.3s ease;
    }

    .form-group input:focus {
      border-color: #ff6600;
    }

    .checkbox {
      display: flex;
      align-items: flex-start;
      margin-bottom: 20px;
      font-size: 14px;
      color: #555;
      line-height: 1.4;
    }

    .checkbox input {
      margin-right: 10px;
      accent-color: #ff6600;
      margin-top: 2px;
    }

    .checkbox a {
      color: #ff6600;
      text-decoration: none;
    }

    .checkbox a:hover {
      text-decoration: underline;
    }

    .btn {
      background: #ff6600;
      color: #fff;
      border: none;
      padding: 14px;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
      width: 100%;
      transition: background 0.3s ease;
    }

    .btn:hover {
      background: #e65c00;
    }

    .image-box {
      flex: 1;
      background: url('C:\Users\intel\OneDrive\Desktop\image.jpg') no-repeat center center/cover;
      min-height: 300px;
    }

    /* Mobile Responsive */
    @media (max-width: 768px) {
      .container {
        flex-direction: column;
      }

      .image-box {
        height: 250px;
      }

      .form-box {
        padding: 20px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Form Section -->
    <div class="form-box">
      <h2>Register</h2>
      <p>Hello everyone.</p>

      <form action="#" method="post">
        <div class="form-group">
          <input type="text" placeholder="First Name" required>
          <input type="text" placeholder="Last Name" required>
        </div>

        <div class="form-group">
          <input type="email" placeholder="Email Address" required>
        </div>

        <div class="form-group">
          <input type="tel" placeholder="+00 0000 000 0000">
          <input type="url" placeholder="Website (optional)">
        </div>

        <div class="form-group">
          <input type="password" placeholder="Password" required>
          <input type="password" placeholder="Confirm Password" required>
        </div>

        <div class="checkbox">
          <input type="checkbox" required>
          <label>
            Creating an account means you're okay with our 
            <a href="#">Terms and Conditions</a> and our 
            <a href="#">Privacy Policy</a>.
          </label>
        </div>

        <button class="btn" type="submit">Register</button>
      </form>
    </div>

    <!-- Image Section -->
    <div class="image-box"></div>
  </div>
</body>
</html>
