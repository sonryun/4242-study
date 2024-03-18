# 다섯번째 문제
<p>-자신의 이름으로 만든 객체 리터럴 안에 다른 객체 리터럴을 만든 후 버튼을 클릭했을 때 
  프로퍼티가 동적 생성되고 alert창에 값이 도출되는 코드를 추가한다.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quiz5</title>

    <style>
        body {
            margin: 300px 400px;
        }
        button {
            width: 170px;
            height: 40px;
        }
    </style>
</head>
<body>
    <button onclick="studentId1()">나의 학번은?</button>
    <button onclick="major1()">나의 전공은?</button>
    <button onclick="gender1()">나의 성별은?</button>
    <button onclick="compliment1()">나에게 해주고 싶은 말은?</button>

    <script>
        const son = {
            school: {
                studentId: 202310468,
                major: '의료정보과'
            },
            gender: '여'
        };

        function compliment1() {
            son.compliment = '안녕';
            alert(son.compliment);
        }

        function studentId1() {
            alert(son.school.studentId);
        }

        function major1() {
            alert(son.school['major']);
        }

        function gender1() {
            alert(son['gender']);
        }
    </script>
</body>
</html>
```
