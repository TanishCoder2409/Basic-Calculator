# Basic-Calculator
This repository contains the HTML , CSS, and JavaScript code i used to develop a basic Calculator that can perform arithmetic operations
<br>
HTML CODE:
<html>
<title>JavaScript Project</title>
<head>
<link rel="stylesheet" href="calc.css">
<script src="calculator.js"></script>
</head>
<body>
<div id="calc">
<input type="text" id="displayresult">
<button onclick="display(1)" id="n1">1</button>
<button onclick="display(2)" id="n2">2</button>
<button onclick="display(3)" id="n3">3</button>
<button onclick="display(4)" id="n4">4</button>
<button onclick="display(5)" id="n5">5</button>
<button onclick="display(6)" id="n6">6</button>
<button onclick="display(7)" id="n7">7</button>
<button onclick="display(8)" id="n8">8</button>
<button onclick="display(9)" id="n9">9</button>
<button onclick="display(0)" id="n0">0</button>
<button onclick="display('+')" id="plus">+</button>
<button onclick="display('-')" id="minus">-</button>
<button onclick="display('/')" id="divide">/</button>
<button onclick="display('*')" id="multiply">*</button>
<button onclick="cleartext()" id="clear">C</button>
<button onclick="calcresult()" id="equals">=</button>
</div>
</body>
</html>
<br>
CSS CODE:
body{
background-color:#f4f4f4;
display:flex;
align-items:center;
justify-content:center;
}
#calc{
background-color:white;
border:1px solid black;
border-radius:10px;
width:242px;
height:280px;
box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
border:none;
}
#n1{
border:1px solid #ddd;
width:50px;
font-weight:700;
font-size:1.2em;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
background-color:#ddd;
font-family:helvetica;
}
#temp{
height:50px;
width:230px;
border:1px solid #ddd;
background-color:rgb(210,210,210,0.25);
margin:5px 5px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
}
#n2{
border:1px solid #ddd;
background-color:#ddd;
width:50px;
font-weight:700;
font-size:1.2em;
font-family:helvetica;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
left:60px;
bottom:55px;
}
#n3{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
font-family:helvetica;
width:50px;
font-weight:700;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
left:120px;
bottom:110px;
}
#n4{
font-size:1.2em;
font-family:helvetica;
border:1px solid #ddd;
font-weight:700;
background-color:#ddd;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:110px;
}
#n5{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
font-weight:700;
font-family:helvetica;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:165px;
left:60px;
}
#n6{
font-size:1.2em;
font-weight:700;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
font-family:helvetica;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:220px;
left:120px;
}
#n7{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
font-family:helvetica;
font-weight:700;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:220px;
}
#n8{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
font-weight:700;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
font-family:helvetica;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:275px;
left:60px;
}
#n9{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
font-family:helvetica;
font-weight:700;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:330px;
left:120px;
}
#n0{
font-size:1.2em;
font-weight:700;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
font-family:helvetica;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:330px;
}
#plus{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
font-family:helvetica;
border-top-left-radius:5px;
font-weight:700;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:550px;
left:180px;
}
#minus{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
font-weight:700;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
font-family:helvetica;
align-items:center;
justify-content:center;
position:relative;
bottom:550px;
left:180px;
}
#divide{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
font-weight:700;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
font-family:helvetica;
position:relative;
bottom:550px;
left:180px;
}
#multiply{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
font-weight:700;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
font-family:helvetica;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:550px;
left:180px;
}
#clear{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
display:flex;
align-items:center;
justify-content:center;
font-family:helvetica;
position:relative;
bottom:605px;
left:60px;
background:#dc3545;
color:white;
}
#equals{
font-size:1.2em;
border:1px solid #ddd;
background-color:#ddd;
width:50px;
height:50px;
border-top-left-radius:5px;
border-top-right-radius:5px;
border-bottom-left-radius:5px;
border-bottom-right-radius:5px;
margin:5px 5px;
font-family:helvetica;
display:flex;
align-items:center;
justify-content:center;
position:relative;
bottom:660px;
background:#28a745;
color:white;
left:120px;
}
#divide:active{
background: #bbb;
}
#multiply:active{
background: #bbb;
}
#minus:active{
background: #bbb;
}
#plus:active{
background: #bbb;
}
#equals:active{
background: #bbb;
}
#n0:active{
background: #bbb;
}
#n1:active{
background: #bbb;
}
#n2:active{
background: #bbb;
}
#n3:active{
background: #bbb;
}
#n4:active{
background: #bbb;
}
#n5:active{
background: #bbb;
}
#n6:active{
background: #bbb;
}
#n7:active{
background: #bbb;
}
#n8:active{
background: #bbb;
}
#n9:active{
background: #bbb;
}
#clear:active{
background: #bbb;
}
#displayresult{
    width: 100%;
    height: 50px;
    font-size: 1.5em;
    padding: 5px;
    border: 1px solid #ddd;
    border-radius: 5px;
    outline:none;
    background-color:rgb(210,210,210,0.25);
}
<br>
JavaScript Code:
function display(input){
    let variable=document.querySelector("#displayresult");
    variable.value=variable.value+input;
}
function cleartext(){
    let variable=document.querySelector("#displayresult");
    variable.value="";
}
function calcresult(){
    let variable=document.querySelector("#displayresult");
    variable.value=eval(variable.value);
}
