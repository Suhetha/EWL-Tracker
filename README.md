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
  }
   </script>
   </form>
</body>
</html>
body{
    margin:0;
    padding:0;
    font-family:sans-serif;
    background:url('https://images.squarespace-cdn.com/content/v1/5ea237e587e03021f9ef8cc2/1591632715798-GZ810CZ0DMW3J0HD2ODF/Group-members.jpg?format=500w');
    background-size:cover;
    }
    
    .box{
    height:40%;
    width:40%;
    padding:30px;
    position:absolute;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    background:aquamarine;
    text-align:center;
    }
    .box h1{
    color:black;
    text-tranform:uppercase;
    font-weight:700;
    }
    .box input[type="text"],.box input[type="password"]
{
    background:none;
    display:block;
    margin:20px auto;
    text-align:center;
    border:3px solid blue;
    padding:14px ;
    width:220px;
    color:white;
    border-radius:24px;
    }
    .box input[type="text"]:focus,.box input[type="password"]:focus
    {
    width:270px;
    border-color:rgb(248, 248, 245)
}
.box input[type="submit"]
{
border:0;	
background:black;
display:inline-block;
margin:25px auto;
text-align:center;
border: 6px;px solid black;
padding:14px 25px;
outline:none;
color:red;
border-radius:20px;
cursor:pointer;
}

