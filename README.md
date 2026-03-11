<!DOCTYPE html>
<html>

<head>
<title>uglyfoid wired node</title>

<style>
body{
background:black;
color:#00ff88;
font-family:Courier New, monospace;
text-align:center;
}

h1{
color:#00ff88;
text-shadow:0 0 10px #00ff88;
}

a{
color:#00ff88;
text-decoration:none;
}
</style>

</head>

<body>

<h1>WELCOME TO THE WIRED</h1>

<p>present day. present time.</p>

<a href="#">logs</a><br>
<a href="#">network</a>

</body>

</html>    );
    pointer-events:none;
}

/* title */

h1{
    margin-top:80px;
    font-size:40px;
    color:#00ff88;
    text-shadow:0 0 5px #00ff88, 0 0 20px #00ff88;
}

/* subtitle */

.subtitle{
    color:#00cc66;
    margin-bottom:40px;
}

/* wired terminal box */

.box{
    border:1px solid #00ff88;
    width:320px;
    margin:auto;
    padding:20px;
    background:rgba(0,0,0,0.6);
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
    animation:blink 1s infinite;
}

@keyframes blink{
    0%{opacity:1;}
    50%{opacity:0;}
    100%{opacity:1;}
}

</style>
</head>

<body>

<h1>WELCOME TO THE WIRED</h1>

<p class="subtitle">present day • present time</p>

<div class="box">

<p>> user: guest</p>
<p>> access node: uglyfoid network</p>

<br>

<a href="logs.html">logs</a>
<a href="network.html">network</a>
<a href="about.html">about</a>

</div>

<br>

<p>> connection stable<span class="cursor">_</span></p>

</body>
</html>
