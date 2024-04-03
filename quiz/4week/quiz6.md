# 여섯번째 문제
<p>-입력받은 두 수 합을 제곱하는 프로그램 만들기.</p>

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        function add(x, y) {
            return x + y;
        }

        function square(num) {
            return num * num;
        }

        function addsquare(x, y) {
            var adds = add(x, y);
            return square(adds);
        }

        var num1 = prompt('첫 번째 수를 입력하세요');
        var num2 = prompt('두 번째 수를 입력하세요');

        num1 = parseInt(num1);
        num2 = parseInt(num2);

        var result = addsquare(num1, num2);
        alert('두 숫자의 합의 제곱' + result);
    </script>
</body>
</html>
```
