# 네번째 문제
<p>-메모를 입력하고 저장하는 프로그램. 이때, 저장 버튼을 누르면  메모가 저장되었습니다.
  라는 알림창이 뜨고 지우기 버튼을 누르면 다시 리셋되어 메모를 다시 작성할 수 있다.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quiz4</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: lightgoldenrodyellow;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 600px;
        }
    
        .container {
            text-align: center;
        }
    
        textarea {
            width: 300px;
            height: 200px;
            padding: 10px;
            margin-bottom: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
            resize: none;
            box-sizing: border-box;
        }
    
        button {
            background-color: #f8ff6c;
            color: rgb(27, 125, 0);
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.2s;
        }
    
        button:hover {
            background-color: #eaff00;
        }
    </style>
    </head>
    <body>
    
    <div class="container">
        <textarea id="memo" placeholder="메모를 입력하세요"></textarea>
        <br>
        <button onclick="saveMemo()">저장</button>
        <button onclick="clearMemo()">지우기</button>
    </div>
    
    <script>
        function saveMemo() {
            alert('메모가 저장되었습니다');
        }

        function clearMemo() {
            var clear = document.getElementById("memo");
            clear.value = '';
        }
    </script>
    
    </body>
    </html>
```
