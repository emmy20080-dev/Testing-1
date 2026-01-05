# Testing-1
For Winners Who Never Sell Low
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>$CHAD — Built for Winners</title>

<meta name="description" content="$CHAD is a Solana meme token built for strong holders, viral culture, and dominance.">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Inter',sans-serif}
body{background:radial-gradient(circle at top,#0f1f1a,#050807);color:#fff;line-height:1.6}
a{text-decoration:none;color:inherit}
.container{max-width:1200px;margin:auto;padding:80px 20px}
nav{display:flex;justify-content:space-between;align-items:center;padding:20px 40px}
nav h1{color:#19f6b2;font-weight:800}
.btn{background:#19f6b2;color:#000;padding:12px 24px;border-radius:10px;font-weight:700;transition:.3s}
.btn:hover{transform:translateY(-3px);box-shadow:0 10px 30px rgba(25,246,178,.4)}

.hero{text-align:center;padding:120px 20px}
.hero h2{font-size:52px;font-weight:800;margin-bottom:20px}
.hero p{max-width:800px;margin:auto;opacity:.9}

.hero-buttons a{margin:10px;display:inline-block}

.fade{opacity:0;transform:translateY(40px);transition:all .8s ease}
.fade.show{opacity:1;transform:none}

.card{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:16px;padding:40px;margin-top:40px}

.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:30px;text-align:center}
.stat h3{font-size:42px;color:#19f6b2}

iframe{width:100%;height:520px;border:none;border-radius:14px}

.nfts{display:flex;gap:20px;overflow-x:auto}
.nfts img{width:260px;border-radius:16px;opacity:.8}

footer{text-align:center;padding:40px;opacity:.6}

@media(max-width:768px){
.hero h2{font-size:38px}
}
</style>
</head>

<body>

<nav>
<h1>$CHAD</h1>
<a class="btn" href="https://t.me/chadt0ken">Get Started</a>
</nav>

<section class="hero">
<h2>$CHAD — Built for Winners Who Never Sell Low</h2>
<p>No gimmicks. No weak hands. Just pure Chad energy.</p>
<div class="hero-buttons">
<a class="btn" href="https://t.me/chadt0ken">🚀 Join Community</a>
<a class="btn" href="#">📈 View Chart</a>
</div>
</section>

<section class="container fade">
<h3>Live Stats</h3>
<div class="stats">
<div class="stat">
<h3 class="count" data-target="1000">0</h3>
<p>Holders Target</p>
</div>
<div class="stat">
<h3 class="count" data-target="5">0</h3>
<p>Roadmap Phases</p>
</div>
<div class="stat">
<h3 class="count" data-target="100">0</h3>
<p>Community Energy</p>
</div>
</div>
</section>

<section class="container card fade">
<h3>DexScreener</h3>
<p>Live chart will appear here after launch.</p>
<iframe src="https://dexscreener.com/solana"></iframe>
</section>

<section class="container fade">
<h3>Chad NFT Collection (Preview)</h3>
<div class="nfts">
<img src="https://via.placeholder.com/260x260?text=CHAD+NFT+1">
<img src="https://via.placeholder.com/260x260?text=CHAD+NFT+2">
<img src="https://via.placeholder.com/260x260?text=CHAD+NFT+3">
</div>
</section>

<footer>
© 2026 $CHAD — Meme token. DYOR.
</footer>

<script>
// Fade animation
const faders=document.querySelectorAll('.fade');
const obs=new IntersectionObserver(e=>{
e.forEach(x=>x.isIntersecting&&x.target.classList.add('show'))
},{threshold:.2});
faders.forEach(el=>obs.observe(el));

// Counter animation
const counters=document.querySelectorAll('.count');
counters.forEach(counter=>{
const update=()=>{
const target=+counter.dataset.target;
const current=+counter.innerText;
const inc=target/80;
if(current<target){
counter.innerText=Math.ceil(current+inc);
setTimeout(update,30);
}else{counter.innerText=target;}
};
update();
});
</script>

</body>
</html>
