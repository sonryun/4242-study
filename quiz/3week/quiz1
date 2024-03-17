#첫번째 문제
<p>-3개의 문제 버튼을 만들고 버튼을 눌렀을 때 그에 해당하는 문제 창을 띄운다음 
  문제의 빈칸에 맞는 답을 입력하고 맞으면 '정답입니다' 틀리면 '틀렸습니다' 창을 띄운다.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quiz1</title>

    <style>
        body {
            text-align: center;
        }
    </style>
</head>
<body>
    <h3>다음 문제의 빈칸에 알맞은 말을 쓰세요.</h3>
<button id="btn1" onclick="btn_1()">C++과 자바는 클래스 기반 객체지향 언어이다.</button>
<button id="btn2" onclick="btn_2()">프로퍼티는 객체의 상태를 나타내는 값이다.</button>
<button id="btn3" onclick="btn_3()">자바스크립트 함수는 객체이고, 함수는 값으로 취급이 가능하다.</button>

<script>
    function btn_1() {
        var answer = prompt("그렇다면 자바스크립트는 어떤 언어인가요?");
        
        if (answer === '프로토타입 기반 객체지향 언어') {
            alert("정답입니다~");
        } else {
            alert ("틀렸습니다");
        }
    }

    function btn_2() {
        var answer = prompt("그렇다면 프로퍼티는 *와 *로 구성되나요?");
        
        if (answer === '키와 값') {
            alert("정답입니다~");
        } else {
            alert ("틀렸습니다");
        }
    }

    function btn_3() {
        var answer = prompt("이 말은 곧 **** 값으로 사용 가능하다는 말입니다.");

        if (answer === '프로퍼티') {
            alert("정답입니다~");
        } else {
            alert ("틀렸습니다");
        }
    }
</script>
</body>
</html>
```
