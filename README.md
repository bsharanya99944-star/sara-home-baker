<!DOCTYPE html>
<html>
<head>
<title>Sara Home Baker | Menu</title>

<style>
body{
    margin:0;
    font-family: Georgia, serif;
    background:#fdecef;
    color:#5a4a42;
    overflow-x: hidden;
    position: relative;
}

/* Sections */
.section{
    padding:50px 20px;
    text-align:center;
}

.card{
    background:#fff;
    max-width:900px;
    margin:auto;
    padding:40px;
    border-radius:20px;
    box-shadow:0 10px 25px rgba(0,0,0,0.1);
}

h1{
    font-size:42px;
    color:#7a4a3a;
    margin-bottom:10px;
}

h2{
    color:#7a4a3a;
    margin-bottom:30px;
}

p{
    line-height:1.7;
}

.menu{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.item{
    background:#fff7f8;
    padding:15px;
    border-radius:15px;
    box-shadow:0 5px 10px rgba(0,0,0,0.08);
}

.price{
    color:#c0392b;
    font-weight:bold;
}

.footer{
    margin-top:30px;
    font-size:14px;
}

.divider{
    margin:50px auto;
    width:60%;
    height:2px;
    background:#e3bcbc;
}

/* 🌸 Sprinkles / Confetti */
.sprinkle {
    position: fixed;           
    width: 15px;              /* heart size */
  height: 15px;
    top: -20px;
    opacity: 0.9;
    animation: fall linear infinite;
    z-index: 9999;
	background: red;           /* default color, JS will override */
    
}

/* Keyframes for falling + rotation + slight drift */
@keyframes fall {
    0% {
        transform: translateY(0) translateX(0) rotate(0deg);
        opacity: 1;
    }
    100% {
        transform: translateY(110vh) translateX(30px) rotate(360deg);
        opacity: 0;
    }
}
</style>
</head>

<body>

<!-- 🌸 WELCOME PAGE -->
<div class="section">
    <div class="card">
        <h1>சாரா<br>Home Baker</h1>
        <p><b>Welcome to Our Sweet World!</b></p>
        <p>
            AT SARA HOME BAKER, EVERY BITE IS MADE WITH LOVE,
            FRESH INGREDIENTS, AND A SPRINKLE OF JOY.
            WHETHER YOU’RE HERE FOR OUR SOFTEST CUPCAKES,
            RICH BROWNIES, OR BUTTERY COOKIES,
            WE’RE DELIGHTED TO SERVE YOU.
        </p>
        <h3><b>THANK YOU FOR SUPPORTING OUR SMALL BUSINESS.</b></h3>

        <div class="footer">
            📸 @sara_home_baker <br>
            FSSAI: 22425558000199
        </div>
    </div>
</div>

<div class="divider"></div>

<!-- 🍰 MENU PAGE -->
<div class="section">
    <h2>SARA HOME BAKERY – MENU</h2>
    <div class="menu">
        <div class="item">Chocolate Cake<br><span class="price">₹750</span></div>
        <div class="item">Dream Cake(250 g)<br><span class="price">₹300</span></div>
        <div class="item">Vanilla Cake<br><span class="price">₹740</span></div>
        <div class="item">Chocolate Oreo<br><span class="price">₹850</span></div>
        <div class="item">Rasmalai Cake<br><span class="price">₹1040</span></div>
        <div class="item">Small Jar Cake<br><span class="price">₹50</span></div>
        <div class="item">Choco Vanilla<br><span class="price">₹750</span></div>
        <div class="item">Pineapple Cake<br><span class="price">₹875</span></div>
        <div class="item">Gulab Jamun Cake<br><span class="price">₹870</span></div>
        <div class="item">KitKat Cake<br><span class="price">₹900</span></div>
        <div class="item">Choco Lava Cake (1pc)<br><span class="price">₹35</span></div>
        <div class="item">White Forest Cake<br><span class="price">₹900</span></div>
        <div class="item">Chocolate Cupcake (1pc)<br><span class="price">₹30</span></div>
        <div class="item">Vanilla Cupcake (1pc)<br><span class="price">₹20</span></div>
        <div class="item">Cookies (½ kg)<br><span class="price">₹350</span></div>
        <div class="item">Brownies (½ kg)<br><span class="price">₹380</span></div>
        <div class="item">Red Velvet Cake<br><span class="price">₹980</span></div>
        <div class="item">Chocolate Truffle Cake<br><span class="price">₹1230</span></div>
        <div class="item">Brownies (1pc)<br><span class="price">₹40</span></div>
        <div class="item">Tres leches cake (250g)<br><span class="price">₹340</span></div>
        <div class="item">Bento cakes (250 g)<br><span class="price">₹ depends on the flavor</span></div>
        <div class="item">Rainbow cake<br><span class="price">₹900</span></div>
        <div class="item">Butterscotch cake<br><span class="price">₹1300</span></div>
        <div class="item">Muttamittai (½ kg)<br><span class="price">₹350</span></div>
        <div class="item">Tea cake (1pc)<br><span class="price">₹20</span></div>
        <div class="item">Rose milk cake<br><span class="price">₹820</span></div>
        <div class="item">Coffee cake<br><span class="price">₹850</span></div>
        <div class="item">Marble tea cake(1PC)<br><span class="price">₹30</span></div>
        <div class="item">Honey cake(1PC)<br><span class="price">₹35</span></div>
        <div class="item">Tub cake (250g)<br><span class="price">₹300</span></div>
        <div class="item">Orange tea cake(1PC)<br><span class="price">₹25</span></div>
        <div class="item">Ferrero Rocher Cake<br><span class="price">₹1330</span></div>
    </div>

    <div class="footer">
       <h1>“100% HOMEMADE  200% HAPPINESS”</h1>
       <br>
       @sara_home_baker
    </div>
</div>

<!-- 🌸 JS for colorful sprinkles -->
<script>
const colors = ['#ff6b6b','#ffde7d','#ffe2e2','#ffb3b3','#fff0b3']; // pastel cake colors
const sprinkleCount = 60;

for(let i=0; i<sprinkleCount; i++){
    let s = document.createElement('div');
    s.className = 'sprinkle';
    s.style.left = Math.random() * window.innerWidth + 'px';
    s.style.width = s.style.height = (5 + Math.random()*8) + 'px';
    s.style.background = colors[Math.floor(Math.random()*colors.length)];
    s.style.animationDuration = (3 + Math.random()*4) + 's';
    s.style.animationDelay = Math.random() * 5 + 's'; // stagger start
    document.body.appendChild(s);
}
</script>

</body>
</html>
