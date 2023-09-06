# glowing-validation-form
<!DOCTYPE html>
<head>
<title>Login page</title>
<center>
<h1>Login</h1>
<style>
h1{
  color:white;
  height:100%;
  width:100%;
}
body{
 display:flex;
 justify-content:center;
 align-items:center;
 min-height:100vh;
 background-image:url("wp7915427.webp");
 
}
.btn{
    padding:8px 20px;
    border-radius:0;
    overflow:hidden;
}
.btn::before{
    position:absolute;
    content:"";
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:linear-gradient(120deg,transparent,var(--primary-color));
    transform:translate(-100%);
    transition:0.6s;
}
.btn:hover{
    background:transparent;
    box-shadow:0 0 20px 10px rgba(51,152,219,0.5);
}
.btn:hover::before{
    transform:translateX(100%);
}
.form-input-material{
 --input-default-border-color:white;
 --input-border-bottom-color:white;
}
.form-input-material input{
  color:black;
}
.login-form{
   display:flex;
   flex-direction:column;
   align-items:center;
   padding:50px 40px;
   color:white;
   background:rgba(0,0,0,0.8);
   border-radius:10px;
   box-shadow:0 0.4px 0.4px rgba(128,128,128,0.109);
}
.login-form h1{
   margin:0 0 24px 0;
}
.login-form .form-input-material{
   margin:12px 0;
}
.login-form .btn{
  width:100%;
  margin:18px 0 9px 0;
}
</style>
</head>
<body>
<form class="login-form"action="javascript:void(0);">
<div class="form-input-material">
<input type="text" name="username" id="username"
placeholder="username"autocomplete="off" class="form-control-material"required/>
<label for="username">username</label>
</div>
<div class="form-input-material">
<input type="password" name="password" id="password" placeholder="password" autocomplete="off" class="form-control-material" required/>
<label for="password">password</label>
</div>
<button type="submit" class="btn btn-primary btn-ghost">login</button>
</form>
</center>
</body>
</html>
