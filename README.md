# ISHMAEL
TO YOUU❤️❤️❤️
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Love 💘</title>

<style>
body{
    margin:0;
    padding:0;
    font-family: 'Arial', sans-serif;
    background: linear-gradient(135deg,#ff758c,#ff7eb3);
    overflow:hidden;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    color:white;
    text-align:center;
}

.container{
    width:90%;
    max-width:700px;
    background: rgba(255,255,255,0.15);
    padding:40px;
    border-radius:25px;
    backdrop-filter: blur(10px);
    box-shadow:0 0 30px rgba(0,0,0,0.2);
    animation:fadeIn 1s ease;
}

.slide{
    display:none;
    animation:fadeIn 1s ease;
}

.active{
    display:block;
}

button{
    margin-top:25px;
    padding:15px 35px;
    border:none;
    border-radius:30px;
    background:white;
    color:#ff4f81;
    font-size:18px;
    cursor:pointer;
    font-weight:bold;
    transition:0.3s;
}

button:hover{
    transform:scale(1.08);
}

.emoji{
    font-size:55px;
    animation:float 2s infinite;
}

.floating{
    position:absolute;
    font-size:25px;
    animation:rise 6s linear infinite;
    opacity:0.7;
}

@keyframes rise{
    0%{
        transform:translateY(100vh);
        opacity:0;
    }
    100%{
        transform:translateY(-120vh);
        opacity:1;
    }
}

@keyframes fadeIn{
    from{opacity:0; transform:translateY(20px);}
    to{opacity:1; transform:translateY(0);}
}

@keyframes float{
    0%{transform:translateY(0);}
    50%{transform:translateY(-10px);}
    100%{transform:translateY(0);}
}

h1{
    font-size:40px;
}

p{
    font-size:22px;
    line-height:1.7;
}
</style>
</head>

<body>

<div class="container">

<div class="slide active">
<div class="emoji">💘</div>
<h1>Hey Love🥹</h1>
<p>
I know i’m one person you hate and the least person you wanna hear from right now...
but look🥹 I created this for you to cheer you up and say...
</p>
<h1>“I’M SORRY”💔</h1>
<button onclick="nextSlide()">Next 💗</button>
</div>

<div class="slide">
<div class="emoji">🥺</div>
<p>
If i had a chance to say it in person...
I would hold you close🤍
kiss you on your forehead💋
and whisper in your ears that...
</p>
<h1>“I LOVE YOU”❤️</h1>
<button onclick="nextSlide()">Next 😻</button>
</div>

<div class="slide">
<div class="emoji">🌒</div>
<p>
I will be waiting for you to come back🥹
so we can fix our mistakes,
make each other happy again,
forever and always💘
from the moon🌒 and backkk.
</p>
<button onclick="nextSlide()">Next 💞</button>
</div>

<div class="slide">
<div class="emoji">🤣</div>
<p>
And noo noo noo waittt🤣🤣🤣
Not yettt you silly head😹
</p>
<p>
For me to send the next surprise...
send me this heart:
</p>

<h1>💗</h1>

<p>
You don’t have to type anything🥹
because i know you’re mad my love
and i respect that.
</p>

<h2>I’m really really sorryyyy🥹💔</h2>

<button onclick="nextSlide()">Final Surprise 💝</button>
</div>

<div class="slide">
<div class="emoji">💖</div>
<h1>Forever Yours ❤️</h1>

<p>
No matter what happens...
you will always have a special place in my heart🥹
</p>

<h1>💘💘💘</h1>

<p>
Thank you for opening this little surprise😻
</p>
</div>

</div>

<script>
let currentSlide = 0;
const slides = document.querySelectorAll('.slide');

function nextSlide(){
    slides[currentSlide].classList.remove('active');
    currentSlide++;
    slides[currentSlide].classList.add('active');
}

function createHeart(){
    const heart = document.createElement('div');
    heart.classList.add('floating');
    heart.innerHTML = ['💖','💘','🥹','💗','😻','❤️'][Math.floor(Math.random()*6)];

    heart.style.left = Math.random()*100 + 'vw';
    heart.style.fontSize = (20 + Math.random()*30) + 'px';

    document.body.appendChild(heart);

    setTimeout(()=>{
        heart.remove();
    },6000);
}

setInterval(createHeart,500);
</script>

</body>
</html>
