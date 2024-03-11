# free vps rdp 6h
<h1>COMING SOON...</h1>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flying Dots</title>
<link rel="stylesheet" href="styles.css">
</head>
  <style>
    body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #f0f0f0;
}

.dot-container {
  display: flex;
}

.dot {
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background-color: #333;
  margin: 5px;
  animation: fly 2.5s infinite alternate;
}

@keyframes fly {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(0);
  }
}
    </style>
<body>
<div class="dot-container">
  <div class="dot"></div>
  <div class="dot"></div>
  <div class="dot"></div>
</div>
</body>
</html>
