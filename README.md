
<!-- 
Online HTML, CSS and JavaScript editor to run code online.
-->
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="style.css" />
  <title>Browser</title>
</head>

<body>
<div class="scene">
  <div class="character">
    <div class="face"></div>
    <div class="eye"></div>
    <div class="eye"></div>
    <div class="eyebrow"></div>
    <div class="eyebrow"></div>
    <div class="nose"></div>
    <div class="mouth"></div>
  </div>
</div>
</body>
  
  <style> 
  .scene {
  perspective: 800px;
}

.character {
  position: relative;
  transform-style: preserve-3d;
  animation: spin 3s linear infinite;
}

@keyframes spin {
  from {
    transform: rotateY(0deg);
  }
  to {
    transform: rotateY(360deg);
  }
}

.face {
  position: absolute;
  width: 200px;
  height: 200px;
  background-color: #F5A623;
  border-radius: 50%;
}

.eye {
  position: absolute;
  width: 25px;
  height: 25px;
  background-color: #fff;
  border-radius: 50%;
  top: 75px;
}

.eye:nth-child(1) {
  left: 60px;
}

.eye:nth-child(2) {
  right: 60px;
}

.eyebrow {
  position: absolute;
  width: 50px;
  height: 10px;
  background-color: #333;
  top: 45px;
}

.eyebrow:nth-child(1) {
  left: 55px;
  transform: rotate(-15deg);
}

.eyebrow:nth-child(2) {
  right: 55px;
  transform: rotate(15deg);
}

.nose {
  position: absolute;
  width: 10px;
  height: 10px;
  background-color: #333;
  border-radius: 50%;
  top: 85px;
  left: 80px;
}

.mouth {
  position: absolute;
  width: 50px;
  height: 20px;
  background-color: #333;
  border-radius: 50%;
  bottom: 25px;
  left: 75px;
  transform: rotate(15deg);
}

  </style>

</html>
