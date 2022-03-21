# page-loader

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Document</title>
</head>
<body>
    <div class="middle">
        <div class="bar bar1"></div>
        <div class="bar bar2"></div>
        <div class="bar bar3"></div>
        <div class="bar bar4"></div>
        <div class="bar bar5"></div>
        <div class="bar bar6"></div>
    </div>
</body>
</html>


body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background: #000;
}
.middle {
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  position: absolute;
}
.bar {
  width: 10px;
  height: 70px;
  background: #fff;
  display: inline-block;
  transform-origin: bottom center;
  border-top-right-radius: 20px;
  border-top-left-radius: 20px;
  /*   box-shadow:5px 10px 20px inset rgba(255,23,25.2); */
  animation: loader 2.2s linear infinite;
}
.bar1 {
  animation-delay: 0.1s;
}
.bar2 {
  animation-delay: 0.2s;
}
.bar3 {
  animation-delay: 0.3s;
}
.bar4 {
  animation-delay: 0.4s;
}
.bar5 {
  animation-delay: 0.5s;
}
.bar6 {
  animation-delay: 0.6s;
}

@keyframes loader {
  0% {
    transform: scaleY(0.1);
    background: ;
  }
  25% {
    transform: scaleY(0.5);
    background: rgb(17, 230, 176);
  }
  50% {
    transform: scaleY(0.1);
    background: transparent;
  }
  75% {
    transform: scaleX(-0.1);
    background: transparent;
  }
  100% {
    transform: scaleX(-0.5);
    background: crimson;
  }
}
