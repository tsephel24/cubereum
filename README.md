# cubereum
1.cubereum.html


<html>
<head>
<title>Login and Registration Form design</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
 
  <div class="login-page">
    <div class="form">
      <form class="register-form">
      <input type="text" placeholder="Username" maxlength="11" minLength="5"/ pattern="[a-zA-Z][a-zA-Z0-9-_.]11}">
      <input type="Password" placeholder="Password" maxlength="12"  minlength="8" />
      <input type="Email" placeholder="Email ID" maxlength="40"/>

      <button>Create</button>
      <p class="message">Already registered? <a href="#">Login</a>
      </p>
    </form>
    <form class="login-form">
    <input type="text" placeholder="Username" maxlength="11" minLength="5"/ pattern="[a-zA-Z][a-zA-Z0-9-_.]11}">
    <input type="Password" placeholder="Password" maxlength="12"  minlength="8" />
    <button>login</button>
    <p class="message">Not registered? <a hrf="#"> Register</a></p>
  </form>
  </div>
</div>
<script src='https://code.jquery.com/jquery-3.3.1.min.js'></script>
<script>
$('.message a').click(function(){
$('form').animate({height:"toggle", opacity: "toggle"}, "slow");
});
</script>
</body>
</html>


2.style.css
body{
    background-image: linear-gradient(rgba(0,0,0,0.6),rgba(0,0,0,0.6)),url(potala.jpg);
    height:100vh;
    background-size: cover;
    background-position: center;
}
.login-page{
  width: 360px;
  padding: 10% 0 0;
  margin: auto;
}

.form{
  position:relative;
  z-index: 1;
  background: rgba(7, 40, 195, 0.8);
  max-width: 360px;
  margin: 0 auto 100px;
  padding: 45px;
  text-align: center;
}

.form input{
  font-family: "Roboto", sans-serif;
  outline: 1;
  background: #f2f2f2;
  width: 100%
  border: 0;
  margin: 0 0 15px;
  padding: 15px;
  box-sizing: border-box;
  font-size: 15px;
}

.form button{
  font-family: "Roboto", sans-serif;
  text-transform: uppercase;
  outline: 0;
  background: #4CAF50;
  width: 100%;
  border: 0;
  padding: 15px;
  color:#FFFFFF;
  font-size: 15px;
  cursor: pointer;
}

.form button:hover,.form button:active{
  background: #43A047;
}

.form .message{
  margin: 15px 0 0;
  color: aliceblue;
  font-size: 12px;
}

.form .message a{
  color: #4CAF50;
  text-decoration: none;
}
.form .register-form{
  display: none;
}  



 
