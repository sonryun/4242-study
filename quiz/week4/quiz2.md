# 두번째 문제
<p>-문자를 입력하고 입력한 문자열을 뒤집기</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>너의 글자를 다 뒤집겠어!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            max-width: 300px;
            margin: 50px auto;
            text-align: center;
        }
        input[type="text"] {
            width: 100%;
            padding: 10px;  
            margin-bottom: 10px; 
            box-sizing: border-box;
            border-radius: 10px;
            background-color: rgb(186, 235, 242);
        }
        button {
            padding: 10px 20px; 
            background-color: rgb(248, 209, 213);
            border-radius: 10px;
            color: #000000;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #c9f938;
        }
        #result {    
            margin-top: 20px;
        }
    </style>
    </head>
    <body>
    
    <div class="container">
        <h2>문자를 입력하세요.</h2>
        <input type="text" id="inputString" placeholder="지금 가장 보고싶은 사람에게 한마디">
        <button onclick="reverseString()">뒤집어집니다.</button>
        <div id="result"></div>
    </div>
    
    <script>
        function reverseString() {   
            var inputString = document.getElementById("inputString").value;
            var reversedString = inputString.split('').reverse().join('');
            document.getElementById("result").innerText = '뒤집어서 보세요:' + reversedString;
        }
    </script>
    
    </body>
    </html>
```
