![image](https://user-images.githubusercontent.com/66727050/152101390-84f85ae9-f74c-4baa-b70a-788545d03c81.png)

# Solution:

## index.html

<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="css/buttonsGrid.css" type="text/css">
    <title>Buttons Grid</title>
</head>

<body>
    <div id="btns">
        <button class="btn" id="btn1" value="1">1</button>
        <button class="btn" id="btn2" value="2">2</button>
        <button class="btn" id="btn3" value="3">3</button>
        <button class="btn" id="btn4" value="4">4</button>
        <button class="btn" id="btn5" value="5">5</button>
        <button class="btn" id="btn6" value="6">6</button>
        <button class="btn" id="btn7" value="7">7</button>
        <button class="btn" id="btn8" value="8">8</button>
        <button class="btn" id="btn9" value="9">9</button>
    </div>
    <script>
        btn1 = document.getElementById("btn1");
        btn2 = document.getElementById("btn2");
        btn3 = document.getElementById("btn3");
        btn4 = document.getElementById("btn4");
        btn5 = document.getElementById("btn5");
        btn6 = document.getElementById("btn6");
        btn7 = document.getElementById("btn7");
        btn8 = document.getElementById("btn8");
        btn9 = document.getElementById("btn9");
        btn5.addEventListener('click', function () {
            var btn1V = btn1.value;
            btn1.innerHTML = btn4.innerHTML;
            btn1.value = btn4.innerHTML;
            btn4.innerHTML = btn7.innerHTML;
            btn4.value = btn7.innerHTML;
            btn7.innerHTML = btn8.innerHTML;
            btn7.value = btn8.innerHTML;
            btn8.innerHTML = btn9.innerHTML;
            btn8.value = btn9.innerHTML;
            btn9.innerHTML = btn6.innerHTML;
            btn9.value = btn6.innerHTML;
            btn6.innerHTML = btn3.innerHTML;
            btn6.value = btn3.innerHTML;
            btn3.innerHTML = btn2.innerHTML;
            btn3.value = btn2.innerHTML;
            btn2.innerHTML = btn1V;
            btn2.value = btn1V;
        });
    </script>
</body>

</html>

## buttonsGrid.css

#btns {
    width                : 75%;
}

.btn {
    width    : 30%;
    height   : 48px;
    font-size: 24px;
}
