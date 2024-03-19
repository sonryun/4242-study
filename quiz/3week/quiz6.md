# 여섯번째 문제
<p>-투두 리스트를 입력하고 출력하는 프로그램. 텍스트 입력 창에 할 일을 입력한 후 '추가' 버튼을 누르면 화면에 입력한 할 일이 출력된다.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>투두 리스트 만들기</title>
  <style>
    .container {
      width: 400px;
      height: 500px;
      background-color: #dbddf9;
      padding: 10px;
      text-align: center;
    }

    input {
      text-align: center;
      width: 250px;
      height: 30px;
      font-size: 17px;
    }

    button {
      width: 50px;
      height: 33px;
    }

    #list {
      text-align: left;
      font-size: 17px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>오늘의 할 일</h1>
    <input
      type="text"
      id="inputList"
      placeholder="오늘의 할 일을 입력하세요"
    />
    <button onclick="addList()">추가</button>
    <ul id="list"></ul>
  </div>

  <script>
    const toDoList = document.querySelector('#list');

    function addList() {
      const inputList = document.getElementById('inputList').value.trim();

      if (inputList !== '') {
        const newItem = document.createElement('li');
        newItem.textContent = inputList;

        toDoList.appendChild(newItem);

        document.getElementById('inputList').value = '';
      } else {
        alert('할 일을 입력하세요.');
      }
    }
  </script>
</body>
</html>
```

<h5>새로 안 것</h5>
<b>trim()함수:</b> 문자열의 양 끝에서 공백을 제거한 새로운 문자열을 반환하는 함수.
<br>
<b>createElement():</b> 문서 안에 괄호 안에 있는 요소를 만든다는 의.
<br>
<b>appendChild()함수:</b> 지정된 부모 노드에 자식 노드를 추가하는 메소드.
