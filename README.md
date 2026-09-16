# PROJETO.CAROLINA
index.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Angela</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    background: black;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
  }
  .heart {
    position: relative;
    width: 280px;
    height: 280px;
    background: red;
    transform: rotate(-45deg);
    animation: pulse 1.2s infinite;
    box-shadow: 0 0 40px red;
  }
  .heart::before,
  .heart::after {
    content: "";
    position: absolute;
    width: 280px;
    height: 280px;
    background: red;
    border-radius: 50%;
  }
  .heart::before { top: -140px; left: 0; }
  .heart::after { left: 140px; top: 0; }

  .heart span {
    position: absolute;
    transform: rotate(45deg);
    left: 35px;
    top: 65px;
    width: 280px;
    text-align: center;
    color: white;
    font-family: Arial, sans-serif;
    font-size: 48px;
    font-weight: bold;
    z-index: 10;
  }

  @keyframes pulse {
    0% { transform: rotate(-45deg) scale(1); }
    50% { transform: rotate(-45deg) scale(1.1); }
    100% { transform: rotate(-45deg) scale(1); }
  }
</style>
</head>
<body>
  <div class="heart">
    <span>Angela</span>
  </div>
</body>
</html>
