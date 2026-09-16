# PROJETO.CAROLINA
index.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Festa da Angela - Ilê Asé Três Irmãos</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@600;700&family=Pacifico&display=swap');
  *{margin:0; padding:0; box-sizing:border-box;}
  body{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    font-family:'Fredoka', sans-serif;
    background: linear-gradient(180deg, #ffe4e6 0%, #fecdd3 50%, #fda4af 100%);
    padding:20px;
    overflow:hidden;
  }
  .coracao{ position:fixed; top:-40px; animation: cair linear infinite; z-index:1; }
  @keyframes cair{ 0%{transform:translateY(-10vh) scale(0.5)} 100%{transform:translateY(110vh) scale(1.2)} }

  .card{
    width:100%;
    max-width:460px;
    background:white;
    border-radius:40px;
    overflow:hidden;
    box-shadow:0 20px 60px rgba(225,29,72,0.3);
    border:5px solid #f43f5e;
    position:relative;
    z-index:2;
  }
  .topo{
    background: linear-gradient(180deg, #f43f5e 0%, #e11d48 100%);
    padding:30px 15px;
    text-align:center;
  }
  .topo h1{
    color:white;
    font-size:14px;
    letter-spacing:2px;
    opacity:0.9;
  }
  .nome{
    font-family:'Pacifico', cursive;
    font-size:72px;
    color:white;
    line-height:1;
    text-shadow: 3px 3px 0 #881337, 0 0 20px rgba(255,255,255,0.6);
    margin:10px 0;
    animation: pulsa 1.2s infinite;
  }
  @keyframes pulsa{ 0%,100%{transform:scale(1)} 50%{transform:scale(1.08)} }

  .conteudo{ padding:28px 24px; text-align:center; }

  .titulo-festa{
    font-size:30px;
    color:#e11d48;
    line-height:1;
  }
  .titulo-festa span{
    display:block;
    font-size:16px;
    background:#ffe4e6;
    color:#be123c;
    padding:8px 15px;
    border-radius:50px;
    margin-top:10px;
  }

  .coracoes{ font-size:40px; letter-spacing:15px; margin:10px 0; animation: brilha 1s infinite alternate; }
  @keyframes brilha{ from{transform:scale(1)} to{transform:scale(1.1)} }

  .info{
    background:#fff1f2;
    border:3px dotted #fb7185;
    border-radius:22px;
    padding:16px;
    margin-top:18px;
    text-align:left;
    font-size:14.5px;
    color:#4c0519;
    line-height:1.6;
  }
  .info b{ color:#e11d48; }

  .btn{
    display:block;
    width:100%;
    margin-top:14px;
    padding:16px;
    border-radius:50px;
    text-decoration:none;
    font-weight:700;
    font-size:18px;
    text-align:center;
    transition:0.1s;
  }
  .btn-rosa{ background:#f43f5e; color:white; box-shadow:0 6px 0 #be123c; }
  .btn-azul{ background:#3b82f6; color:white; box-shadow:0 6px 0 #1d4ed8; }
  .btn:active{ transform:translateY(6px); box-shadow:none; }
  .footer{ background:#ffe4e6; padding:12px; font-size:11px; color:#e11d48; text-align:center; }
</style>
</head>
<body>

<script>
  let cors=['💖','💗','💓','💞','❤️','💕'];
  for(let i=0;i<35;i++){
    let c=document.createElement('div');
    c.className='coracao';
    c.innerHTML=cors[Math.floor(Math.random()*cors.length)];
    c.style.left=Math.random()*100+'vw';
    c.style.fontSize=(18+Math.random()*28)+'px';
    c.style.animationDuration=(3+Math.random()*5)+'s';
    c.style.animationDelay=Math.random()*5+'s';
    document.body.appendChild(c);
  }
</script>

<div class="card">
  <div class="topo">
    <h1>ILÊ ASÉ TRÊS IRMÃOS CONVIDA</h1>
    <div class="nome">Angela 💖</div>
    <div style="background:white; color:#e11d48; display:inline-block; padding:6px 18px; border-radius:30px; font-size:13px; font-weight:700;">📅 24 DE OUTUBRO • 19H</div>
  </div>

  <div class="conteudo">
    <div class="coracoes">💖✨💖</div>
    <div class="titulo-festa">
      FESTA DE
      IBEJADA E BAIANOS
      <span>🍬 Com muito amor e axé 💕</span>
    </div>

    <p style="font-size:14px; color:#6b7280; margin-top:12px;">
      Uma festa feita com todo carinho<br>
      para celebrar com a nossa querida <b>Angela</b>
    </p>

    <div class="info">
      <p>💖 <b>Homenageada:</b> Angela</p>
      <p>📍 <b>Local:</b> Ilê Asé Três Irmãos</p>
      <p>🏠 Rua Anésia Molino Ribeiro<br>
      &nbsp;&nbsp;&nbsp;&nbsp;Vila Isis Cristina, Embu das Artes - SP<br>
      &nbsp;&nbsp;&nbsp;&nbsp;CEP: 06815-480</p>
      <p>👗 <b>Venha:</b> De coração aberto e roupa clara</p>
    </div>

    <a class="btn btn-rosa" href="https://wa.me/5511999999999?text=Oi%20Angela!%20Confirmo%20presença%20na%20sua%20festa%20dia%2024.10%20💖" target="_blank">💖 CONFIRMAR PRESENÇA</a>
    <a class="btn btn-azul" href="https://www.google.com/maps/search/?api=1&query=Rua+Anésia+Molino+Ribeiro+Vila+Isis+Cristina+Embu+das+Artes" target="_blank">📍 VER NO MAPA</a>
  </div>

  <div class="footer">Feito com 💖 para Angela • Ilê Asé Três Irmãos • Axé!</div>
</div>

</body>
</html>
