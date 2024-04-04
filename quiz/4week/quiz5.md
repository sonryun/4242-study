# 다섯번째 문제
<p>-1부터 45까지의 숫자 중에서 6개를 무작위로 선택하여 보여주는 로또 번호 생성기 만들기.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>로또 번호 생성기</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
</style>
</head>
<body>
<h1>♣로또 번호 생성기♣</h1>
<p>다음주에 학교 안 나오면 그렇게 알아라... </p>
<p id="lottoNumbers"></p>
<button onclick="result()">두근두근...♡///</button>

<script>
var lottoNumbers = [];

function result() {
    lottoNumbers = [];

    for (var i = 1; i <= 45; i++) {
        lottoNumbers.push(i);
    }

    var selectedNumbers = [];

    for (var i = 0; i < 6; i++) {
    var random = Math.floor(Math.random() * 45);

    var selectedNumber = lottoNumbers[random];
    selectedNumbers.push(selectedNumber);
}

    selectedNumbers.sort(function(a, b) {
        return a - b;
    });

    var lottoNumbersText = selectedNumbers.join(', ');
    document.getElementById('lottoNumbers').textContent = "추첨된 로또 번호: " + lottoNumbersText;
}
</script>
</body>
</html>
```
