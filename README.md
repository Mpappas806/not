<html>
<body>
    <a href="#" onclick="clickCounter()"><img src="https://lh3.googleusercontent.com/proxy/CkZmZzYwliy-ABDeCsW-UBwnepINeXO9oPHLmocjEq4EOQYIffwx-tCPQ529cJL6W4zV2bmKPkNipkoJWXM3vKy6_32YFy7Hbxgqi8vQ-ckdCrZrXrg-bl_jR4rhL7aS" alt="Cookie PNG Transparent Images | PNG All"/></a>
    <a href="#" onclick="resetCounter()">Reset Counter</a>
    <br>
    <p id="result"></p>

    <script>
    function clickCounter() {
        var count = localStorage.clickcount = Number(localStorage.clickcount)+1;
        if (isNaN(count) === true) {
            count = localStorage.clickcount = 1;
            document.getElementById("result").innerHTML = count;
        } else {
            document.getElementById("result").innerHTML = count;
        }
    } 

    function resetCounter() {
        var reset = localStorage.clickcount = 0;
        document.getElementById("result").innerHTML = reset;
    }
   </script>
</body>
</html>
