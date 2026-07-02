<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>花畑の朝</title>
<style>
  html, body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    overflow-x: hidden;
    font-family: "Hiragino Sans", "Yu Gothic", sans-serif;
  }

  .stage {
    position: relative;
    width: 100%;
    aspect-ratio: 960 / 540;
    overflow: hidden;
  }

  .bg {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  .title {
    position: absolute;
    top: 6%;
    left: 4%;
    color: #e6437a;
    font-weight: bold;
    line-height: 1.6;
    font-size: clamp(14px, 2.6vw, 26px);
    background: rgba(255, 255, 255, 0.55);
    padding: 0.5em 0.8em;
    border-radius: 8px;
  }

  .butterfly {
    position: absolute;
    width: 60px;
    z-index: 5;
  }

  .butterfly1 {
    top: 60%;
    left: 20%;
    animation: fly1 9s ease-in-out infinite;
  }

  .butterfly2 {
    top: 70%;
    left: 55%;
    width: 45px;
    animation: fly2 7s ease-in-out infinite;
  }

  .butterfly3 {
    top: 65%;
    left: 75%;
    width: 50px;
    animation: fly3 11s ease-in-out infinite;
  }

  @keyframes fly1 {
    0%   { transform: translate(0, 0) rotate(0deg); }
    25%  { transform: translate(30px, -20px) rotate(5deg); }
    50%  { transform: translate(60px, 5px) rotate(-3deg); }
    75%  { transform: translate(20px, 25px) rotate(4deg); }
    100% { transform: translate(0, 0) rotate(0deg); }
  }

  @keyframes fly2 {
    0%   { transform: translate(0, 0) rotate(0deg); }
    30%  { transform: translate(-25px, -15px) rotate(-6deg); }
    60%  { transform: translate(-45px, 10px) rotate(4deg); }
    100% { transform: translate(0, 0) rotate(0deg); }
  }

  @keyframes fly3 {
    0%   { transform: translate(0, 0) rotate(0deg); }
    20%  { transform: translate(15px, -25px) rotate(3deg); }
    50%  { transform: translate(-20px, -10px) rotate(-5deg); }
    80%  { transform: translate(10px, 15px) rotate(2deg); }
    100% { transform: translate(0, 0) rotate(0deg); }
  }
</style>
</head>
<body>

  <div class="stage">
    <img src="bg0.png" alt="花畑の朝の風景" class="bg">

    <div class="title">
      ぽかぽか陽気の穏やかな朝<br>
      花畑では、蝶々がのんびり飛んでいます
    </div>

    <img src="butterfly.gif" alt="蝶々" class="butterfly butterfly1">
    <img src="butterfly.gif" alt="蝶々" class="butterfly butterfly2">
    <img src="butterfly.gif" alt="蝶々" class="butterfly butterfly3">
  </div>

</body>
</html>
