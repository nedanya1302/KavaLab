# KavaLab
Наша кав’ярня — це місце, де поєднуються якісна кава, смачні страви та сучасний підхід до обслуговування. Ми пропонуємо широкий вибір напоїв і десертів, а також зручний онлайн-калькулятор замовлення, який допоможе швидко розрахувати вартість вашого вибору. Насолоджуйтесь атмосферою затишку та контролюйте своє замовлення в кілька кліків.
<!-- Сайт розроблено студентом Дмитро Усовом, група ФЕМП 4-14 -->
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>KavaLab - Головна</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<header>
  <h1>KavaLab</h1>
  <nav>
    <a href="index.html">Головна</a>
    <a href="menu.html">Меню</a>
    <a href="calculator.html">Калькулятор</a>
    <a href="about.html">Про нас</a>
  </nav>
</header>

<main>
  <h2>Ласкаво просимо до KavaLab</h2>
  <p>Сучасна кав’ярня з онлайн-калькулятором замовлення.</p>
  <p>Email: KavaLab@gmail.com</p>
  <p>Телефон: +380111111111</p>
</main>

<footer>
  <p>Усов Дмитро | ФЕМП 4-14</p>
</footer>

</body>
</html>


<!-- MENU PAGE -->

<!-- Сайт розроблено студентом Дмитро Усовом, група ФЕМП 4-14 -->
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Меню</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<header>
  <h1>KavaLab</h1>
  <nav>
    <a href="index.html">Головна</a>
    <a href="menu.html">Меню</a>
    <a href="calculator.html">Калькулятор</a>
    <a href="about.html">Про нас</a>
  </nav>
</header>

<main>
  <h2>Меню</h2>
  <ul>
    <li>Еспресо - 50 грн</li>
    <li>Капучино - 70 грн</li>
    <li>Лате - 80 грн</li>
    <li>Чай - 40 грн</li>
    <li>Круасан - 60 грн</li>
  </ul>
</main>

<footer>
  <p>Усов Дмитро | ФЕМП 4-14</p>
</footer>
</body>
</html>


<!-- CALCULATOR PAGE -->

<!-- Сайт розроблено студентом Дмитро Усовом, група ФЕМП 4-14 -->
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Калькулятор</title>
  <link rel="stylesheet" href="styles.css">
  <script src="script.js" defer></script>
</head>
<body>
<header>
  <h1>KavaLab</h1>
  <nav>
    <a href="index.html">Головна</a>
    <a href="menu.html">Меню</a>
    <a href="calculator.html">Калькулятор</a>
    <a href="about.html">Про нас</a>
  </nav>
</header>

<main>
  <h2>Калькулятор замовлення</h2>

  <div class="item">Еспресо (50 грн): <input type="number" id="espresso" value="0"></div>
  <div class="item">Капучино (70 грн): <input type="number" id="cappuccino" value="0"></div>
  <div class="item">Лате (80 грн): <input type="number" id="latte" value="0"></div>
  <div class="item">Чай (40 грн): <input type="number" id="tea" value="0"></div>
  <div class="item">Круасан (60 грн): <input type="number" id="croissant" value="0"></div>

  <button onclick="calculate()">Порахувати</button>
  <h3 id="total">Сума: 0 грн</h3>
</main>

<footer>
  <p>Усов Дмитро | ФЕМП 4-14</p>
</footer>
</body>
</html>


<!-- ABOUT PAGE -->

<!-- Сайт розроблено студентом Дмитро Усовом, група ФЕМП 4-14 -->
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Про нас</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<header>
  <h1>KavaLab</h1>
  <nav>
    <a href="index.html">Головна</a>
    <a href="menu.html">Меню</a>
    <a href="calculator.html">Калькулятор</a>
    <a href="about.html">Про нас</a>
  </nav>
</header>

<main>
  <h2>Про нас</h2>
  <p>KavaLab — це кав’ярня нового формату з інтерактивним меню.</p>
</main>

<footer>
  <p>Усов Дмитро | ФЕМП 4-14</p>
</footer>
</body>
</html>


/* STYLES.CSS */
body {
  font-family: Arial;
  margin: 0;
  background: #e0f7f7;
}

header {
  background: #009688;
  color: brown;
  padding: 15px;
  text-align: center;
}

nav a {
  margin: 10px;
  color: brown;
  text-decoration: none;
  font-weight: bold;
}

main {
  padding: 20px;
}

button {
  background: #00bcd4;
  color: brown;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
}

footer {
  background: #009688;
  color: brown;
  text-align: center;
  padding: 10px;
}


// SCRIPT.JS
function calculate() {
  let total = 0;
  total += document.getElementById('espresso').value * 50;
  total += document.getElementById('cappuccino').value * 70;
  total += document.getElementById('latte').value * 80;
  total += document.getElementById('tea').value * 40;
  total += document.getElementById('croissant').value * 60;

  document.getElementById('total').innerText = 'Сума: ' + total + ' грн';
}
