# Rainbow
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .box {
            width: 100%;
            height: 40px;
            background-color: aliceblue;
            border: 1px solid black;
        }
    </style>
</head>
<body>
    <span style="font-size: 30px; color: red;">R</span>
    <span style="font-size: 30px; color: rgb(30, 232, 141);">A</span>
    <span style="font-size: 30px; color: blue;">I</span>
    <span style="font-size: 30px; color: black;">N</span>
    <span style="font-size: 30px; color: purple;">B</span>
    <span style="font-size: 30px; color: #df11bd;">O</span>
    <span style="font-size: 30px; color: rgb(16, 157, 213);">W</span>


    <div class="box" id="box1" onmouseover="changeColor(this)" onmouseout="resetColor(this)">V</div>
    <div class="box" id="box2" onmouseover="changeColor(this)" onmouseout="resetColor(this)">I</div>
    <div class="box" id="box3" onmouseover="changeColor(this)" onmouseout="resetColor(this)">B</div>
    <div class="box" id="box4" onmouseover="changeColor(this)" onmouseout="resetColor(this)">G</div>
    <div class="box" id="box5" onmouseover="changeColor(this)" onmouseout="resetColor(this)">Y</div>
    <div class="box" id="box6" onmouseover="changeColor(this)" onmouseout="resetColor(this)">O</div>
    <div class="box" id="box7" onmouseover="changeColor(this)" onmouseout="resetColor(this)">R</div>

    <script>
        const colors = {
            'v': 'violet',
            'i': 'indigo',
            'b': 'blue',
            'g': 'green',
            'y': 'yellow',
            'o': 'orange',
            'r': 'red',
            'w': 'skyblue'
        };

        function changeColor(element) {
            const color = colors[element.textContent.toLowerCase()];
            if (color) {
                element.style.backgroundColor = color;
            }
        }

        function resetColor(element) {
            element.style.backgroundColor = 'aliceblue';
        }
    </script>
</body>
</html>



