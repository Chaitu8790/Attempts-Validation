 var attempt = 3;

 function att() {

    var user = document.getElementById("name").value;
    var passw = document.getElementById("pwd1").value;
    var namereg = new RegExp(/^[A-Za-z]+$/);
    var passwordreg = new RegExp(/^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*])(?=.{8,})/);
    if (namereg.test(user) && passwordreg.test(passw)) {
       alert("Login success");
       window.open('https://www.google.co.in', '_blank', 'toolbar=yes,scrollbars=yes,resizable=yes,top=500,left=500,width=400,height=400');
       return false;

    } else {
       attempt--; // Decrementing by one.
       alert("You have left " + attempt + " attempt;");
       check();
       // Disabling fields after 3 attempts.
       if (attempt == 0) {
          document.getElementById("name").disabled = true;
          document.getElementById("pwd1").disabled = true;
          document.getElementById("sub").disabled = true;
          return false;
       }
    }

 }

 function check() {

    var user = document.getElementById('name').value;
    var passw = document.getElementById('pwd1').value;
    var namereg = new RegExp(/^[A-Za-z]+$/);
    var passwordreg = new RegExp(/^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*])(?=.{8,})/);

    if (user == "") {

       document.getElementById('fnm').innerHTML = "*Please enter name";
       document.getElementById('name').focus();
       document.getElementById('fnm').style.color = " red";
       return false;
    } else if (!namereg.test(user)) {
       document.getElementById('fnm').innerHTML = "*Name must be in characters only";
       document.getElementById('name').focus();
       document.getElementById('fnm').style.color = "red";
       return false;
    } else if (user.length < 6) {
       document.getElementById('fnm').innerHTML = "*Please enter at least 6 characters";
       document.getElementById('name').focus();
       document.getElementById('fnm').style.color = "red";
       return false;
    } else {
       document.getElementById('name').style.backgroundColor = "white";
       document.getElementById('fnm').style.display = "none";
    }

    if (passw == "") {
       document.getElementById('pd').innerHTML = "*Please enter password";
       document.getElementById('pwd1').focus();
       document.getElementById('pd').style.color = "red";
       return false;
    } else if (!passwordreg.test(passw)) {
       document.getElementById('pd').innerHTML = "*Please enter valid password";
       document.getElementById('pwd1').focus();
       document.getElementById('pd').style.color = "red";
       return false;
    } else {
       document.getElementById('pd').innerHTML = "*Please enter correct password";
       document.getElementById('pwd1').style.backgroundColor = "white";
       document.getElementById('pd').style.display = "none";
       return false;
    }

 }