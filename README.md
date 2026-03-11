<!DOCTYPE html>
<html>

<head>
<title>uglyfoid wired node</title>

<style>

body{
background:black;
color:#00ff88;
font-family:"Courier New", monospace;
text-align:center;
margin:0;
padding:0;
overflow-x:hidden;
}

/* CRT scanlines */

body::after{
content:"";
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:repeating-linear-gradient(
to bottom,
rgba(0,0,0,0) 0px,
rgba(0,0,0,0) 2px,
rgba(0,0,0,0.15) 3px
);
pointer-events:none;
}

/* title glow + flicker */

h1{
margin-top:80px;
color:#00ff88;
text-shadow:0 0 5px #00ff88, 0 0 20px #00ff88;
animation:flicker 2s infinite;
}

/* flicker animation */

@keyframes flicker{
0%{opacity:1;}
5%{opacity:0.7;}
10%{opacity:1;}
15%{opacity:0.8;}
20%{opacity:1;}
}

/* typing effect */

.typing{
overflow:hidden;
white-space:nowrap;
border-right:2px solid #00ff88;
display:inline-block;
animation:typing 3s steps(30,end), blink 1s infinite;
}

@keyframes typing{
from{width:0}
to{width:100%}
}

@keyframes blink{
50%{border-color:transparent}
}

/* terminal box */

.box{
border:1px solid #00ff88;
padding:20px;
width:320px;
margin:auto;
background:rgba(0,0,0,0.7);
}

/* links */

a{
display:block;
color:#00ff88;
text-decoration:none;
margin:8px;
}

a:hover{
text-shadow:0 0 10px #00ff88;
}

/* blinking cursor */

.cursor{
animation:cursorblink 1s infinite;
}

@keyframes cursorblink{
0%{opacity:1;}
50%{opacity:0;}
100%{opacity:1;}
}

</style>

</head>

<body>

<h1>WELCOME TO THE WIRED</h1>

<p class="typing">present day • present time</p>

<br><br>

<div class="box">

<p>> user : guest</p>
<p>> access node : uglyfoid network</p>

<br>

<a href="we are.html">logs</a>
<a href="always.html">network</a>
<a href="connected.html">about</a>

</div>

<br>

<p>> connection stable<span class="cursor">_</span></p>

</body>

</html>
