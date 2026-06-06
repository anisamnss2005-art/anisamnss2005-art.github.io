<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>CYBER DRAGON SAMURAI</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#050510;
    overflow:hidden;
    height:100vh;
    color:white;
}

/* Background GIF */
.bg{
    position:fixed;
    width:100%;
    height:100%;
    top:0;
    left:0;
    background:url('https://media.giphy.com/media/l3vRfNA1p0rvhMSvS/giphy.gif');
    background-size:cover;
    opacity:0.15;
    z-index:-3;
}

/* Neon Overlay */
.overlay{
    position:fixed;
    width:100%;
    height:100%;
    background:
    radial-gradient(circle at center,
    rgba(0,255,255,0.2),
    transparent 60%);
    z-index:-2;
}

/* Lightning */
.lightning{
    position:absolute;
    width:100%;
    height:100%;
    background:white;
    opacity:0;
    animation:flash 6s infinite;
    z-index:-1;
}

@keyframes flash{
    0%,90%,100%{opacity:0;}
    91%{opacity:.8;}
    92%{opacity:0;}
    93%{opacity:.6;}
    94%{opacity:0;}
}

/* Content */
.container{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.title{
    font-size:70px;
    font-weight:bold;
    color:#00ffff;
    text-shadow:
    0 0 10px #00ffff,
    0 0 20px #00ffff,
    0 0 40px #00ffff,
    0 0 80px #00ffff;
    animation:pulse 2s infinite;
}

@keyframes pulse{
    50%{
        transform:scale(1.05);
    }
}

.subtitle{
    margin-top:15px;
    font-size:22px;
    color:#d8d8ff;
    text-shadow:0 0 15px #8a2be2;
}

.dragon{
    font-size:80px;
    margin:25px 0;
    animation:float 3s infinite ease-in-out;
}

@keyframes float{
    50%{
        transform:translateY(-20px);
    }
}

.btn{
    margin-top:30px;
    padding:18px 45px;
    border:none;
    border-radius:50px;
    font-size:20px;
    cursor:pointer;
    color:white;
    background:linear-gradient(
    90deg,
    #ff0000,
    #ff8800,
    #ffcc00);
    box-shadow:
    0 0 15px red,
    0 0 30px orange,
    0 0 60px yellow;
    transition:.3s;
}

.btn:hover{
    transform:scale(1.1);
}

.fire{
    position:absolute;
    bottom:0;
    width:100%;
    height:120px;
    background:
    linear-gradient(
    to top,
    #ff3300,
    transparent);
    filter:blur(15px);
    animation:fire 2s infinite alternate;
}

@keyframes fire{
    from{
        height:100px;
    }
    to{
        height:150px;
    }
}

/* Cyber Border */
.border{
    position:absolute;
    inset:15px;
    border:2px solid #00ffff;
    box-shadow:
    0 0 10px #00ffff,
    0 0 25px #00ffff;
    pointer-events:none;
}

</style>
</head>
<body>

<div class="bg"></div>
<div class="overlay"></div>
<div class="lightning"></div>
<div class="fire"></div>
<div class="border"></div>

<div class="container">

    <div class="dragon">🐉⚔️</div>

    <div class="title">
        CYBER SAMURAI
    </div>

    <div class="subtitle">
        NAGA • PETIR • API • NEON • FUTURISTIK
    </div>

    <button class="btn">
        MASUK SEKARANG
    </button>

</div>

</body>
</html>
