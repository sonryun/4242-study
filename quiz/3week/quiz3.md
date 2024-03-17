# 세번째 문제
<p>-객체 리터럴을 활용한 학생 정보 리스트 만들기</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quiz3</title>
</head>
<body>
    <div id="studentInfo"></div>

    <script>
        const student = [
        {
            이름: '손륜',
            나이: 21,
            정보: {
                키: 164,
                시력: -7,
            },
            좋아하는활동: ['탁구', '영화보기'],
            성별: '여성'
        },
        {
            이름: '장철수',
            나이: 24,
            정보: {
                키: 180,
                시력: 0.5,
            },
            좋아하는활동: ['축구', '댄스'],
            성별: '남성'
        },
        {
            이름: '김지민',
            나이: 18,
            정보: {
                키: 159,
                시력: -2.5,
            },
            좋아하는활동: ['미술', '독서'],
            성별: '여성'
        },
        ];

        const studentInfoContainer = document.getElementById('studentInfo'); 

        let studentInfoText = '';
        studentInfoText += '이름: ' + student[0].이름 + ', 나이: ' + student[0].나이 + ', 키: ' + student[0].정보.키 + ', 시력: ' + student[0].정보.시력 + ', 좋아하는 활동: ' + student[0].좋아하는활동.join(', ') + ', 성별: ' + student[0].성별;
        studentInfoText += '이름: ' + student[1].이름 + ', 나이: ' + student[1].나이 + ', 키: ' + student[1].정보.키 + ', 시력: ' + student[1].정보.시력 + ', 좋아하는 활동: ' + student[1].좋아하는활동.join(', ') + ', 성별: ' + student[1].성별;
        studentInfoText += '이름: ' + student[2].이름 + ', 나이: ' + student[2].나이 + ', 키: ' + student[2].정보.키 + ', 시력: ' + student[2].정보.시력 + ', 좋아하는 활동: ' + student[2].좋아하는활동.join(', ') + ', 성별: ' + student[2].성별;
        
        studentInfoContainer.textContent = studentInfoText;
    </script>
</body>
</html>
```
