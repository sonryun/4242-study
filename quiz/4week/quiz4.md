# 네번째 문제
<p>-입력한 연도에 맞춰 해당 선수의 이력이 나오게 하기. 선수들의 평균 나이 구하기.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Runners Literal</title>
  <style>
    body{
      background-color: rgb(255, 255, 147);
    }
    button{
      width: 90px; height: 80px;
    }
    #inputYear{
      border: 1px solid black;
      width: 250px;
    }
  </style>
</head>
<br>
  <button onclick="winner()">수상자 이력 검색</button>
  <input type="text" id="inputYear" placeholder="검색하고 싶으신 연도를 입력하세요">
  <button onclick="ageAvg()">선수들 평균나이는?</button><br>
  <textarea id="textarea" cols="20" rows="10" readonly></textarea>
  
  
  <script>
    const runningArr = [
    {name: '김윤수', age: '17', year: 2023,
    moto: "항상..최선을 다합니다..!"},
    {name: '이지예', age: '18', year: 2022,
      moto: "우승은 내꺼이지예"},
    {name: '김첨지', age: '21', year: 2021,
      moto: "운수가 좋은 날이네요~"},
    {name: '오타니', age: '29', year: 2020,
      moto: "전 달리기도 잘합니다"},
    ]

    function winner() {
      let year = parseInt(document.getElementById("inputYear").value);
      let text = document.getElementById("textarea"); 
      
      if(year === 2020) {
        text.value = JSON.stringify(runningArr[3]);
      } else if(year === 2021) {
        text.value = JSON.stringify(runningArr[2]);
      } else if(year === 2022) {
        text.value = JSON.stringify(runningArr[1]);
      } else if(year === 2023) {
        text.value = JSON.stringify(runningArr[0]);
      } else {
        alert("연도를 다시 입력해주세요.");
      }
    }

    function ageAvg() {
      let sum = 0;

      for (let i = 0; i < runningArr.length; i++) {
        sum += parseInt(runningArr[i].age);
      }
      let ageavg = sum / runningArr.length;
      alert('선수들의 평균 나이는' + ageavg  + '입니다.');
    }
    
  </script>
  
</body>
</html>
```
