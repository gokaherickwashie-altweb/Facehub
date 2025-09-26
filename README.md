<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Face hub</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #2c3e50, #3498db);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .signup-container {
      background: #fff;
      padding: 30px;
      border-radius: 12px;
      width: 350px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.25);
      text-align: center;
    }

    .profile-pic {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid #3498db;
      object-fit: cover;
      margin-bottom: 15px;
    }

    .upload-btn {
      margin-bottom: 20px;
    }

    .signup-container h2 {
      margin-bottom: 20px;
      color: #333;
    }

    .form-group {
      margin-bottom: 15px;
      text-align: left;
    }

    .form-group label {
      font-size: 14px;
      color: #444;
      display: block;
      margin-bottom: 6px;
    }

    .form-group input {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 14px;
      outline: none;
      transition: border 0.3s ease;
    }

    .form-group input:focus {
      border-color: #3498db;
    }

    .signup-btn {
      width: 100%;
      padding: 12px;
      background: #3498db;
      border: none;
      border-radius: 8px;
      color: #fff;
      font-size: 16px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .signup-btn:hover {
      background: #2c80b4;
    }
  </style>
</head>
<body>

  <div class="signup-container">
    <h2>Create Account</h2>
    
    <!-- Profile Picture Upload -->
    <img src="https://via.placeholder.com/120" class="profile-pic" id="preview" alt="Profile Picture">
    <div class="upload-btn">
      <input type="file" accept="image/*" onchange="loadFile(event)">
    </div>

    <!-- Signup Form -->
    <form>
      <div class="form-group">
        <label>Username</label>
        <input type="text" placeholder="Enter username" required>
      </div>

      <div class="form-group">
        <label>Email</label>
        <input type="email" placeholder="Enter email" required>
      </div>

      <div class="form-group">
        <label>Password</label>
        <input type="password" placeholder="Enter password" required>
      </div>

      <div class="form-group">
        <label>City</label>
        <input type="text" placeholder="Enter your city" required>
      </div>

      <button type="submit" class="signup-btn">Sign Up</button>
    </form>
  </div>

  <script>
    // Preview uploaded profile picture
    function loadFile(event) {
      const preview = document.getElementById('preview');
      preview.src = URL.createObjectURL(event.target.files[0]);
    }
  </script>

</body>
</html> # Facehub
Trying to get trust 
