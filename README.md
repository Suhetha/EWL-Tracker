# EWL-Tracker

<html>
<head>
  <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta http-equiv="X-UA-Compatible" content="ie=edge" />
        <title>LOGIN</title>
        <link rel="stylesheet" href="Reallog.css" />
        <link
            href="https://fonts.googleapis.com/css?family=Rubik&display=swap"
            rel="stylesheet"
        />     
</head>
<body>
  <center><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSblwMDvmPQVOW0h15m6nt_QeoatEXqdTER3iddRptibnegHPlv_GJxD1aECaOHQ55RBrQ&usqp=CAU"><h2>Tracker</h2></center>

<fieldset class="box" action="loginpage.html" method="POST">
<h1 style="text-color: "blue"><b>LOGIN</b></h1><br><br><br>
<input type="text" name="" placeholder="username" id="username">
<input type="password" name="" placeholder="password" id="password">
<input type="submit" value="Login" onclick="validate()">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</fieldset>
<script>

window.addEventListener("DOMContentLoaded", function(){
  var password = document.getElementById("password");
  password.addEventListener("input", function(){
    if (password.validity.tooLong || password.validity.tooShort || password.validity.valueMissing) {
      password.setCustomValidity("Password must be of 8 characters.");
      password.reportValidity();
    } else {
      password.setCustomValidity("");
    }
  });
   </script>
   </form>
</body>
</html>
