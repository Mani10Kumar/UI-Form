# UI-Form
In form you may fill name,contact,email,password etc using javascript
<div id="ui">
	<pre>
	Name
	<input placeholder="Name" id=x1>
	<span id="x1"></span>
	Email
	<input placeholder="Email" id=x2>
	<span id="x2"></span>
	Contact
	<input placeholder="Contact" id=x3>
	<span id="x3"></span>
	Password
	<input placeholder="password" id=x4>
	<span id="x4"></span>
	Confirm Password
	<input placeholder="Confirm password" id=x5>
	<span id="x5"></span>
		<button onclick="abc()">submit</button>
	</pre>
</div>
<script type="text/javascript">
	function abc()
	{
		x1=document.querySelector("input#x1").value
		x2=document.querySelector("input#x2").value
		x3=document.querySelector("input#x3").value
		x4=document.querySelector("input#x4").value
		x5=document.querySelector("input#x5").value
		m1=""
		m2=""
		m3=""
		m4=""
		m5=""
		if (x1=="") {m1="name reqired"}
		 if(x2=="") {m2="email is required"}
		 if(x3=="") {m3="contact is required"}
		 if (x4=="") {m4="password is required"}
		 if (x5=="") {m5="Confirm password is required"}
		 	document.querySelector("span#x1").innerHTML=m1
		 document.querySelector("span#x2").innerHTML=m2
		 document.querySelector("span#x3").innerHTML=m3
		 document.querySelector("span#x4").innerHTML=m4
		 document.querySelector("span#x5").innerHTML=m5
	}
</script>
<style type="text/css">
	span
	{
		color: red;
	}
	#ui
	{
		border: 1px solid black;
		width: 20%;
		text-align: left;
		margin-left: 450px;
		padding: 50px;
		background:skyblue;
		color: black;
	}
	button
	{
		background: black;
		color: white;
	}
</style>
