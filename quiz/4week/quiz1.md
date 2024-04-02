# 첫번째 문제
<p>-배열에서 최댓값과 최솟값 비교하기</p>

```html
function MaxOrMin(numbers) {
    if(numbers.trim() === "") {
        alert('숫자를 다시 입력해주세요.');
        return;
    }

    const arr = numbers.split(' ').map(Number);

    let max = arr[0]; 
    let min = arr[0]; 

    for (let i = 0; i < arr.length; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
        else if (arr[i] < min) {
            min = arr[i];
        }
    }

    console.log("최댓값은" + max + "최솟값은" + min);
}

const numbersInput = "10 9 4 5 2";
console.log(MaxOrMin(numbersInput));
```
