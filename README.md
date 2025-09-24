<!DOCTYPE html>
<html>
<head>
  <title>Protected Page</title>
  <meta charset="UTF-8">
  <style>
    body { font-family: Arial, sans-serif; text-align: center; margin-top: 100px; }
    #content { display: none; }
  </style>
</head>
<body>
  <h2>Enter Password to Continue</h2>
  <input type="password" id="password" placeholder="Enter password">
  <button onclick="checkPassword()">Submit</button>

  <div id="content">
    <h1>🎉 Welcome!</h1>
    <p>This is your protected content.</p>
  </div>

  <script>
    function checkPassword() {
      const correctPassword = "mypassword"; // change this
      const input = document.getElementById("password").value;
      if (input === correctPassword) {
        document.getElementById("content").style.display = "block";
      } else {
        alert("Wrong password!");
      }
    }
  </script>
</body>
</html>
