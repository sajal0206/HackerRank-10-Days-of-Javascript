<img src="https://user-images.githubusercontent.com/66727050/151925667-9f627f84-a95b-466e-96c6-d26f5fb53742.png" width="400">
# Solution:
<hr>
## button.css

#btn{
    width: 96px;
    height: 48px;
    font-size: 24px;
}

## index.html

<!-- Enter your HTML code here -->
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <link rel="stylesheet" href="css/button.css">
        <title>Button</title>
    </head>
    <body>
        <button id="btn" type="button">0</button>
        <script>
        let btn = document.getElementById("btn");
let btnV = btn.value+1;
btn.addEventListener('click', function () {
    btn.innerText = btnV++;
});
        </script>
    </body>
</html>

<hr>
