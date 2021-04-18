# frontendDataEncryption
In the spirit of open source software development, I always encourages community code contribution.<br>
This library will help you out as a frontend input data encryption before calling any-other server technologies and decrypt it to server using javascript 

# Environments in which to use crypto.js
 <h6>Browser Support :</h6>
<ul>
  <li>Chrome 16+</li>
  <li>Edge 12+</li>
  <li>Firefox 3.6+</li>
  <li>Internet Explorer 7+</li>
  <li>Safari 4.0+</li>
</ul>

<h6>Also supports Node, browser extensions</h6>

# How to install this library
<h6>No dependency library required, It's a core javascript library</h6>
<h6>Does not required any jquery</h6>
<h6>Only add this file into your project, like</h6>
<p>ex: <code> "<script src ='crypto.js'></script>" </code></p>
<h6>Congratulations, you are successfully installed this library</h6>

# How to use it 

<h6>Use crypto.encryptGenerator  this function for encrypt your data</h6>
<p>ex : <code>crypto.encryptGenerator("your input data", "yourSecretKey");</code></p>
<h6>Use crypto.decryptGenerator function for decrypt your data</h6>
<p>ex : <code> crypto.decryptGenerator("Your Encrypted Data", "yourSecretKey") </code></p>

<h6>"yourSecretKey" this filed is mandatory for data encryption or decryption, & both should be matched</h6>
<h6>Use crypto.createUniqueKey function for random key generation</h6>
<p>ex : <code>crypto.createUniqueKey(32)</code> 32 is a length of string for key generation</p>

# Example :
<h6> Suppose you have a login form and you want your password should encrypted before calling any server technologies, then see the example </h6>
<p>ex: <code>< input type = 'password' name = 'pwd' id = 'userPwd' placeholder = 'Enter Password' ></code></p>
<p><pre>
<script type = 'text/javascript'>
 function encwd(){
     var getPwd = $("#userPwd").val();
     encPwd = crypto.encryptGenerator(getPwd, "yourSecretKey");
     $("#userPwd").val(encPwd);
 }
 </script>
 </pre>
 </p>
