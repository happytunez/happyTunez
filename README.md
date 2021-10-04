
<!DOCTYPE html>
<html>
<head>
	<style type="text/css">
		body{
					background:#06181f;
	color:#31e8ff;
		}
#logind{
   margin: auto;
	width: 50%;
	height: 400px;
	display: none;
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
#logindd{
   margin: auto;
	width: 50%;
	height: 400px;
	
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
.l{
	height: 900px;
}

.carrier{
	z-index: 50;
    box-shadow: 2px 3px 4px rgba(0, 0, 0, 0.4),
	-2px -3px 4px rgba(255, 255, 255, 0.2);
	background: transparent;
	margin-left: 5px;
	align-content: center;
	width: 100%;
	height: 300px;
	color: white;
	
}
@keyframes show{
	from{
		opacity: 0;
	}
	to{
		opacity: 1;
	}
}

.input{
	transition: width 1s linear;
	
	background: transparent;
	text-align: center;
	border: none;
	border-bottom: 1px solid lightgreen;
	
	width: 90%;
	height: 30px;
	color: white;

}
.input:hover{
	width: 70%;
}
#fff:hover{
	width: 90%;
	background: lightgreen;
	border: none;
	color:#06181f;
}
#fff{
  transition: width 0.5s linear;
	background: transparent;
	text-align: center;
	border: 2px solid lightgreen;
	
	width: 90%;
	height: 30px;
	color: white;
}
#eee{
	color:cyan;
	position: relative;
	top: 90px;
}
#eeee{
	color:cyan;
	position: relative;
	top: 10px;
}
/* Tabs, default for laptop/pc*/
@media screen and (max-width: 720px){
      #logind{
   
	width: 100%;
	height: 500px;
	display: none;
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
#logindd{
   
	width: 100%;
	height: 500px;
	
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
.carrier{
	z-index: 50;
    box-shadow: 2px 3px 4px rgba(0, 0, 0, 0.4),
	-2px -3px 4px rgba(255, 255, 255, 0.2);
	background: transparent;
	margin-left: 5px;
	align-content: center;
	width: 100%;
	height: 400px;
	color: white;
	
}
 }

/* phones*/
 @media screen and (max-width: 420px){
      #logind{
   
	width: 100%;
	height: 500px;
	display: none;
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
#logindd{
   
	width: 100%;
	height: 500px;
	
	background:#06180.5f;
	color:#31e8ff;
	z-index: -1;
	transform: translateY(50%);
   animation:show 1s linear;
}
.carrier{
	z-index: 50;
    box-shadow: 2px 3px 4px rgba(0, 0, 0, 0.4),
	-2px -3px 4px rgba(255, 255, 255, 0.2);
	background: transparent;
	margin-left: 5px;
	align-content: center;
	width: 100%;
	height: 400px;
	color: white;
	
}
 }
 
	</style>
	<title>Create Account</title>
</head>
<body>
<div id="loginDiv" >
	<div id="logind" class="dnone">
		
			<div class="carrier">
				<form id="formm" onsubmit="return explore();">
					<h1 style="text-align: center; color: #06181f;text-shadow: -1px -1px 2px white,
	1px 1px 2px rgba(0, 0, 0, 0.8);">Login</h1><br><br>
				<small style="visibility: hidden;">..</small>	<input id="username" class="input" type="text" name="" placeholder="UserName" required><br><br><br>
					
                 <small style="visibility: hidden;">..</small>   <button id="fff">Sign In</button><br>
                     <a id="eee" href="#" onclick="dis();">Dont have an account, Create now</a>
				</form>

			</div>
		
	</div>


<div id="logindd" class="l">
		
			<div class="carrier">
				<form id="form" onsubmit="return exploree();" >
					<h1 style="text-align: center; color: #06181f;text-shadow: -1px -1px 2px white,
	1px 1px 2px rgba(0, 0, 0, 0.8);">Create Account</h1><br><br>
				<small style="visibility: hidden;">..</small>	<input id="uname" class="input" type="text" name="" placeholder="UserName" required><br><br>
				<small style="visibility: hidden;">..</small>	<input id="email"  style="" class="input" type="email" name="" placeholder="Email" required><br><br>
                 <small style="visibility: hidden;">..</small>	<input id="psw"  class="input" type="password" name="" placeholder="Password" required><br><br>
                 <small style="visibility: hidden;">..</small>	<input id="cpsw"  class="input" type="password" name="" placeholder="confirm your password" required><br><br>
                 <small style="visibility: hidden;">..</small>   <button id="fff">Sign Up</button><br>
                     <a id="eeee" href="#" onclick="disl();">Already have an account? Sign in.</a>
				</form>

			</div>
		
	</div>


















</div>

<script type="text/javascript">
	  function exploree() {
    	// body...
    	var uname = document.getElementById("uname");
    	var email = document.getElementById("email");
    	var psw = document.getElementById("psw");
    	var cpsw= document.getElementById("cpsw");
    	var form = document.getElementById("form");
    	//const uppercase = /[A-Z]/g;
    	//const lowercase = /[a-z]/g;
    	//const num = /[0-9]/g;
    	if (uname.value.length == 0) {
    		alert("fill in values");
    	}else if (psw.value.length == 0) {
    		alert("fill in values");
    	}else if (psw.value != cpsw.value) {
    		alert("Passwords don't match");
    	}
    	else{
    		localStorage.setItem('username',uname.value);
            form.setAttribute('action','HappyTunezWebApp.html');
    		alert("Hi, Finish setting up your Profile, for better experience.\ngo to profile now");
    	}
    	
    }
      function explore() {
    	var storedName = localStorage.getItem('username');
    	var formm = document.getElementById('formm');
    	var username = document.getElementById('username');
    	if (username.value !== storedName) {
           alert("user not found");
    	}else{
    		formm.setAttribute('action','HappyTunezWebApp.html');
    		
    	}

    }
    function dis() {
    	// body...
    	var f = document.getElementById("logind").style.display="none";
    	var fe = document.getElementById("logindd").style.display="block";
    	
    }
    function disl() {
    	// body...
    	var f = document.getElementById("logind").style.display="block";
    	var fe = document.getElementById("logindd").style.display="none";
    	
    }
</script>


</body>
</html>
