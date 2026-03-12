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

/* image section */

.wiredpic{
margin-top:40px;
text-align:center;
}

/* image style */

.wiredpic img{
display:block;
margin:auto;
margin-bottom:15px;
box-shadow:0 0 25px #00ff88;
animation:glitch 2s infinite;
}

/* glitch movement */

@keyframes glitch{
0%{transform:translate(0);}
20%{transform:translate(-2px,2px);}
40%{transform:translate(2px,-2px);}
60%{transform:translate(-1px,1px);}
80%{transform:translate(1px,-1px);}
100%{transform:translate(0);}
}

/* flicker text */

.wiredpic p{
animation:flicker 2s infinite;
}

@keyframes flicker{
0%{opacity:1;}
10%{opacity:0.6;}
20%{opacity:1;}
30%{opacity:0.8;}
40%{opacity:1;}
}

/* moving CRT scanlines */

body::before{
content:"";
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
pointer-events:none;
background:repeating-linear-gradient(
to bottom,
rgba(0,0,0,0) 0px,
rgba(0,0,0,0) 2px,
rgba(0,255,136,0.05) 3px
);
animation:scan 8s linear infinite;
}

/* scanline movement */

@keyframes scan{
0%{transform:translateY(-100%);}
100%{transform:translateY(100%);}
}


.wiredpic{
margin-top:40px;
text-align:center;
}

.lainimg{
width:220px;
display:block;
margin:auto;
box-shadow:0 0 20px #00ff88;
}



  .lainterminal{
margin-top:60px;
text-align:center;
font-family:"Courier New", monospace;
color:#00ff88;
}

/* glowing text */
#quotebox{
display:inline-block;
text-align:left;
white-space:pre-wrap;
text-shadow:0 0 8px #00ff88;
}

/* glitch effect when hover */
#quotebox:hover{
animation:glitch 0.2s infinite;
}

@keyframes glitch{
0%{text-shadow:2px 0 red,-2px 0 blue;}
25%{text-shadow:-2px 0 red,2px 0 blue;}
50%{text-shadow:2px 2px red,-2px -2px blue;}
75%{text-shadow:-2px -2px red,2px 2px blue;}
100%{text-shadow:0 0 10px #00ff88;}
}

/* music button style */
#musicbtn{
margin-top:30px;
background:black;
color:#00ff88;
border:1px solid #00ff88;
padding:10px 20px;
font-family:"Courier New", monospace;
cursor:pointer;
transition:0.3s;
}

/* hover glow */
#musicbtn:hover{
box-shadow:0 0 15px #00ff88;
}

/* pulse when playing */
.playing{
animation:pulse 1.5s infinite;
}

@keyframes pulse{
0%{box-shadow:0 0 5px #00ff88;}
50%{box-shadow:0 0 20px #00ff88;}
100%{box-shadow:0 0 5px #00ff88;}
}

  /*wiredguestbook*/

body {
  background: black;
  color: #00ff88;
  font-family: "Courier New", monospace;
  text-align: center;
  margin: 0;
  padding: 20px;
}

.wiredguestbook{
  border:1px solid #00ff88;
  padding:20px;
  margin:50px auto;
  max-width:600px;
  background: rgba(0,0,0,0.85);
  text-align:left;
}

.guestprompt{
  margin-bottom: 10px;
  white-space: pre-line;
  overflow:hidden;
  border-right:2px solid #00ff88;
  animation: typing 5s steps(80,end) forwards, blink 1s infinite;
}

@keyframes typing{
from{width:0}
to{width:100%}
}

@keyframes blink{
50%{border-color:transparent}
}

.wiredguestbook input,
.wiredguestbook textarea{
  width: 100%;
  background: black;
  color: #00ff88;
  border:1px solid #00ff88;
  font-family:"Courier New", monospace;
  margin-bottom:10px;
  padding:5px;
}

.wiredguestbook button{
  background:black;
  color:#00ff88;
  border:1px solid #00ff88;
  padding:5px 10px;
  cursor:pointer;
}

#message p{
  margin:5px 0;
  text-shadow:0 0 3px #00ff88;
  animation:glitch 2s infinite;
}

@keyframes glitch{
0%{transform:translate(0);}
20%{transform:translate(-1px,1px);}
40%{transform:translate(1px,-1px);}
60%{transform:translate(-1px,1px);}
80%{transform:translate(1px,-1px);}
100%{transform:translate(0);}
}


  
/*giscusguestbook*/

.lainguestbook{
margin-top:50px;
text-align:left;
font-family:"Courier New", monospace;
color:#00ff88;
border:1px solid #00ff88;
padding:20px;
background:rgba(0,0,0,0.7);
}

/* terminal typing effect for the prompt */
.guestprompt{
display:inline-block;
white-space:pre-line;
overflow:hidden;
border-right:2px solid #00ff88;
width:0;
animation:guestTyping 6s steps(120,end) forwards, cursor 1s infinite;
}

/* typing animation */
@keyframes guestTyping{
from{width:0}
to{width:450px} /* adjust width for your text */
}

/* cursor blink */
@keyframes cursor{
50%{border-color:transparent}
}

/* hover glitch effect */
.guestprompt:hover{
animation:glitch 0.2s infinite;
}

@keyframes glitch{
0%{text-shadow:2px 0 red,-2px 0 blue;}
25%{text-shadow:-2px 0 red,2px 0 blue;}
50%{text-shadow:2px 2px red,-2px -2px blue;}
75%{text-shadow:-2px -2px red,2px 2px blue;}
100%{text-shadow:0 0 10px #00ff88;}
}

/* guestbox style */
.guestbox{
margin-top:20px;
}


/*secret main site*/
.wirednodes{
margin-top:200px;
text-align:center;
font-family:monospace;
}

.wirednodes a{
display:block;
color:#00ff88;
margin:10px;
text-decoration:none;
}

.wirednodes a:hover{
text-shadow:0 0 8px #00ff88;
}
    



    
</div>

/*surprised */

  #wiredTrigger{
color:#00ff88;
font-family:"Courier New",monospace;
text-align:center;
margin-top:350px;
cursor:pointer;
}

#wiredSecret{
display:none;
background:black;
border:1px solid #00ff88;
padding:20px;
margin:40px auto;
max-width:520px;
}

#terminal{
color:#00ff88;
font-family:"Courier New",monospace;
white-space:pre-wrap;
}

.cursor{
display:inline-block;
width:10px;
background:#00ff88;
margin-left:5px;
animation:blink 1s infinite;
}

@keyframes blink{
0%{opacity:1;}
50%{opacity:0;}
100%{opacity:1;}
}




  
  
</style>


<head>
  <meta charset="UTF-8">
  <title>The Wired</title>
</head>

<body>

<h1>WELCOME TO THE WIRED</h1>

<p class="typing">close the world • close the next</p>

<br><br>

<div class="lainterminal">

<div id="quotebox"></div>

<button id="musicbtn" onclick="toggleMusic()">▶ connect to the wired</button>

<audio id="bgmusic" loop>
  <source src="https://raw.githubusercontent.com/uglyfemcelx/lainiwakura/main/Ghost's%20Cell%20[nDDtWZMziW4].mp3" type="audio/mpeg">
</audio>

</div>

<script>
// quotes array
const quotes = [
"present day",
"present time",
"",
"the wired is not bound by reality",
"people only see what they want to see",
"is the real world really real?",
"remember,",
"everyone is always connected."
];

const box = document.getElementById("quotebox");
let i = 0;
let charIndex = 0;

function typeQuote(){
    if(i < quotes.length){
        let line = quotes[i];
        if(charIndex < line.length){
            box.innerHTML += line.charAt(charIndex);
            charIndex++;
            setTimeout(typeQuote, 50); // typing speed
        } else {
            box.innerHTML += "<br>";
            i++;
            charIndex = 0;
            setTimeout(typeQuote, 400); // pause between quotes
        }
    }
}

typeQuote(); // start typing

// music toggle
let music = document.getElementById("bgmusic");
let btn = document.getElementById("musicbtn");

function toggleMusic(){
    if(music.paused){
        music.play();
        btn.innerHTML = "❚❚ disconnect";
        btn.classList.add("playing");
    } else {
        music.pause();
        btn.innerHTML = "▶ connect to the wired";
        btn.classList.remove("playing");
    }
}
</script>

<center>

<div class="wiredpic">

<img src="https://raw.githubusercontent.com/uglyfemcelx/lainiwakura/main/ee86ae8f568ecdd24f432af7157ca18c.jpg" class="lainimg" width="220">

<p>> connected to the wired</p>

</div>


<div class="box">

<p>> user : guest</p>
<p>> access node : uglyfoid network</p>

<br>
<div class="wirednodes">

<a href="https://uglyfemcelx.github.io/node01/">node_01</a>

<a href="https://uglyfemcelx.github.io/node02/">node_02</a>

<a href="https://uglyfemcelx.github.io/archive/">memory_archive</a>

<a href="https://uglyfemcelx.github.io/deepwired/">deep_layer</a>

</div>


<br>

<a href="https://youtu.be/vsjJhW0FEHE?si=jpNvX0l7pXfAPW7z"> everyone</a>
<a href="https://youtu.be/T0xCK6J1ics?si=-1dIIS7IPgQfzcuX"> always</a>
<a href="https://youtu.be/j0pvoSl2Es0?feature=shared"> connected</a>


</div>

<p>> connection stable<span class="cursor">_</span></p>


<div class="wiredguestbook">
  <p class="guestprompt">
&gt; you have entered the wired<br>
&gt; the wired hears you, leave a trace of yourself<br>
&gt; type a message and it will echo...
  </p>

<input id="username" placeholder="username (optional)">
<textarea id="message" placeholder="leave a signal in the wired"></textarea>
<button onclick="sendMessage()">send</button>

<div id="guestbook"></div>



<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>

<script>
const supabaseUrl = "https://YOUR_PROJECT_ID.supabase.co"
const supabaseKey = "sb_publishable_ey8E8DUKnY7LyjObIhFUMA_z8-d4_U8"

const supabaseClient = supabase.createClient(supabaseUrl, supabaseKey)

async function sendMessage() {
  const username = document.getElementById("username").value || "anonymous"
  const message = document.getElementById("message").value

  if (!message) {
    alert("the wired cannot hear silence...")
    return
  }

  const { error } = await supabaseClient
    .from("message")
    .insert([{ username: username, message: message }])

  if (error) {
    console.log(error)
    alert("connection unstable… fragments detected")
    alert("someone accessed this node before you")
    alert("the wired remembers every visitor")
    alert("your presence has been recorded")
    alert("something is following the signal back")
    alert("the screen flickers… but nothing changed")
    alert("the logs show a second user")
    alert("they are closer than the network suggests")
    alert("you are not browsing alone")
    alert("i'm behind you :)")
  } else {
    document.getElementById("message").value = ""
    loadMessages()
  }
}

  


  
  

async function loadMessages() {
  const { data } = await supabaseClient
    .from("message")
    .select("*")
    .order("created_at", { ascending: false })

  const box = document.getElementById("wiredguestbook")
  box.innerHTML = ""

  data.forEach(msg => {
    const div = document.createElement("div")
    div.innerHTML = "<b>" + msg.username + ":</b> " + msg.message
    box.appendChild(div)
  })
}

loadMessages()
</script>









<div class="lainguestbook">

  <p class="guestprompt">
  > the wired whispers… fragments of thought drift through. do you have an insight, a trace, a warning. leave it here… let it echo in the void.
  </p>

  <div class="guestbox">
    <script src="https://giscus.app/client.js"
        data-repo="uglyfemcelx/TheWired"
        data-repo-id="R_kgDORj1gxg"
        data-category-id="DIC_kwDORj1gxs4C4MTN"
        data-mapping="url"
        data-strict="0"
        data-reactions-enabled="1"
        data-emit-metadata="1"
        data-input-position="top"
        data-theme="preferred_color_scheme"
        data-lang="en"
        crossorigin="anonymous"
        async>
</script>
  </div>

</div>

<br>


</div>

<br>

<div id="wiredTrigger">dive down deeper into the wired…</div>

<div id="wiredSecret">
<pre id="terminal"></pre>
</div>

<script>

const wiredLines = [
"> you’ve wandered deeper into the wired…",
"> fragments of thought flicker past…",
"> something watches. something whispers.",
"> are you still yourself?",
"> or just a signal in the void?"
]

document.getElementById("wiredTrigger").onclick = function(){

document.getElementById("wiredSecret").style.display="block"

let i = 0
let terminal = document.getElementById("terminal")

function typeLine(){
if(i < wiredLines.length){
terminal.innerHTML += wiredLines[i] + "\n"
i++
setTimeout(typeLine, 1200)
}
}

typeLine()

}

</script>

</body>

</html>














