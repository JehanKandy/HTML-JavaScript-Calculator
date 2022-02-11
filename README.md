# HTML-JavaScript-Calculator
HTML JavaScript Calculator<br><br><br>
****** important *********<br>
DON'T COPY THIS CODE<br>
You should go to the cal.html file <br>
and copy that code<br>

BECAUSE<br>
following code for understanding only<br>
it doesn't work correctly<br>
**************************<br><br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css" type="text/css">
    <title>Cal using css alignment</title>
</head>
<body>
    <div class="container">
        <div class="calculator">
            <input type="text" placeholder="0" id="output-result">
                <button class="delete" onclick="del()">DEL</button>
                <button class="clear" onclick="Clear()">CL</button>
                <button class="cal" onclick="display('%')">%</button>
                <button class="cal" onclick="display('/')">/</button>
                <button class="number" onclick="display('7')">7</button>
                <button class="number" onclick="display('8')">8</button>
                <button class="number" onclick="display('9')">9</button>
                <button class="cal" onclick="display('*')">*</button>
                <button class="number" onclick="display('4')">4</button>
                <button class="number" onclick="display('5')">5</button>
                <button class="number" onclick="display('6')">6</button>
                <button class="cal" onclick="display('-')">-</button>
                <button class="number" onclick="display('1')">1</button>
                <button class="number" onclick="display('2')">2</button>
                <button class="number" onclick="display('3')">3</button>
                <button class="cal" onclick="display('+')">+</button>
                <button class="cal" onclick="display('.')">.</button>
                <button class="number" onclick="display('0')">0</button>
                <button class="equal" onclick="Calculate('')">=</button>

                
           
            </div> 
    </div>
 
    <script>
        let outputScreen = document.getElementById('output-result');

        function display(num){
            outputScreen.value += num
        }
        function Calculate(){
            try{
                outputScreen.value = eval(outputScreen.value);
            }
            catch(err){
                alert("Invalid");
            }
        }
        function Clear(){
            outputScreen.value = "";
        }
        function del(){
            outputScreen.value = outputScreen.value.slice(0,-1);
        }

    </script>
</body>
</html>
