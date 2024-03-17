# 두번째 문제
<p>-추가열에 해당하는 버튼 클릭 시 해당하는 요소가 box안에 나타나고 객체에 프로퍼티 추가 및 콘솔로그,
삭제열에 해당하는 버튼 클릭 시 해당하는 요소가 box안에 사라지고 객체에 프로퍼티 삭 및 콘솔로그</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quiz2</title>

    <style>
        .main {
            width: 400px;
            display: flex;
            justify-content: space-evenly;
        }

        .profil {
            text-align: center;
        }

        h1 {
            margin: 0px;
        }

        .box {
            width: 200px; height: 300px;
            border: 1px solid black;
            display: flex;
            flex-direction: column;
            justify-content: space-evenly;
        }

        .name, .age, .hobby, .color {
            font-size: 30px;
            font-weight: 700;
            display: none;
        }

        .plus {
            display: flex;
            flex-direction: column;
            justify-content: space-evenly;
        }

        .minus {
            display: flex;
            flex-direction: column;
            justify-content: space-evenly;
        }

        button {
            width: 70px; height: 40px;
        }

        h2 {
            text-align: center;
            margin: 0;
        }
    </style>
</head>
<body>
    <div class="main">
        <div class="profil">
            <h1>프로필</h1>
            <div class="box">
                <div class="name">손륜</div>
                <div class="age">21살</div>
                <div class="hobby">피아노</div>
                <div class="color">초록색</div>
            </div>
        </div>
        <div class="plus">
            <h2>추가</h2>
            <button class="p_name" onclick="p_btn_name()">이름</button>
            <button class="p_age" onclick="p_btn_age()">나이</button>
            <button class="p_hobby" onclick="p_btn_hobby()">취미</button>
            <button class="p_color" onclick="p_btn_color()">색</button>
        </div>
        <div class="minus">
            <h2>삭제</h2>
            <button class="m_name" onclick="m_btn_name()">이름</button>
            <button class="m_age" onclick="m_btn_age()">나이</button>
            <button class="m_hobby" onclick="m_btn_hobby()">취미</button>
            <button class="m_color" onclick="m_btn_color()">색</button>
        </div>
    </div>

    <script>
        var person = {
            
        };

        document.querySelector('.p_name').addEventListener('click', function p_btn_name() {
            document.querySelector(".name").style.display = 'block'
            person.name = '손륜';
            console.log(person);
        });

        document.querySelector('.p_age').addEventListener('click', function p_btn_age() {
            document.querySelector(".age").style.display = 'block'
            person.age = 21;
            console.log(person);
        });

        document.querySelector('.p_hobby').addEventListener('click', function p_btn_hobby() {
            document.querySelector(".hobby").style.display = 'block'
            person.hobby = '피아노';
            console.log(person);
        });

        document.querySelector('.p_color').addEventListener('click', function p_btn_color() {
            document.querySelector(".color").style.display = 'block'
            person.color = '초록색';
            console.log(person);
        });

        document.querySelector('.m_name').addEventListener('click', function m_btn_name() {
            document.querySelector(".name").style.display = 'none'
            delete person.name;
            console.log(person);
        });

        document.querySelector('.m_age').addEventListener('click', function m_btn_age() {
            document.querySelector(".age").style.display = 'none'
            delete person.age;
            console.log(person);
        });

        document.querySelector('.m_hobby').addEventListener('click', function m_btn_hobby() {
            document.querySelector(".hobby").style.display = 'none'
            delete person.hobby;
            console.log(person);
        });

        document.querySelector('.m_color').addEventListener('click', function m_btn_color() {
            document.querySelector(".color").style.display = 'none'
            delete person.color;
            console.log(person);
        });
    </script>
</body>
</html>
```
