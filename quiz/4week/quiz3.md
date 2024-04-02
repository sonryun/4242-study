# 세번째 문제
<p>-문자열을 입력한 후 버튼을 누르면 문자열을 오름차순으로 정리해주는 코드만들기.</p>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>오름차순으로 정렬하기</title>
    <style>
      .container {
        width: 450px;
        height: 220px;
        border-radius: 30px;
        padding: 5px;
        background-color: #cbcbf9;
        text-align: center;

        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
      }

      #inputStr {
        font-size: 18px;
        padding: 4px;
        margin-bottom: 3px;
      }

      button {
        font-size: 18px;
        font-weight: normal;
        padding: 3px 5px;
      }

      #result {
        width: 420px;
        height: 60px;
        padding: 4px;
        border-radius: 5px;
        border: 3px solid #ffffff;
        font-size: 20px;
        font-weight: bold;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="item"><h1>오름차순으로 정렬하기</h1></div>
      <div class="item">
        <input type="text" id="inputStr" placeholder="입력해주세요." />
        <button onclick="display()">정렬하기</button>
      </div>
      <div class="item"><p id="result"></p></div>
    </div>

    <script>
      function display() {
        var inputstring = document.getElementById("inputStr").value;
        Str = inputstring.split('').sort().join('');
        document.getElementById("result").innerHTML = Str;
      }
    </script>
  </body>
</html>
```
