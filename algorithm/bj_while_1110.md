# [#1110 더하기 사이클](https://www.acmicpc.net/problem/1110)

## 오답
### 1차: 틀렸습니다
* 식 자체를 잘못 씀
* 
```javascript
const readline = require("readline");

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

rl.on("line", (line) => {
  let input = +line;
  let num = input;
  let answer;
  let cycle = 0;
  let isNotSame = true;

  while (isNotSame) {
    let a = +num % 10;
    let b = Math.floor(+num / 10);
    answer = String(a) + String(a + b);
    answer = num;

    console.log(input, answer);

    cycle++;

    if (input === num) break;
  }
  console.log(cycle);

  rl.close();
});

```
### 2차: 메모리 초과
* 터미널에서 제대로 출력 됨.
* 백준에서 채점시 메모리 초과
```javascript
const readline = require("readline");

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

rl.on("line", (line) => {
  let input = [];

  input.push(line);
  let num = +input[0];
  let answer;

  if (num < 10) {
    num *= 10;
  }

  while (true) {
    let a = +num % 10;
    let b = Math.floor(+num / 10);

    answer = String(a) + String((a + b) % 10);
    input.push(answer);

    num = answer;

    if (input[0] == num) {
      console.log(input.length - 1);
      break;
    }
  }

  rl.close();
});
```

### 3차. 메모리 

```javascript
let fs = require("fs");
let input = fs.readFileSync("/dev/stdin").toString();
let num = [];

num.push(input);

let firstInput = +num[0];
let answer;

if (firstInput < 10) {
  firstInput *= 10;
}

while (true) {
  let a = +firstInput % 10;
  let b = Math.floor(+firstInput / 10);

  answer = String(a) + String((a + b) % 10);
  num.push(firstInput);

  firstInput = answer;

  if (num[0] == firstInput) {
    break;
  }
}
console.log(num.length - 1);

fs.close();
```

### n차. 맞았습니다.
```javascript
const readline = require("readline");

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

rl.on("line", (line) => {
  let num = Number(line);
  let cycle = 0;
  let answer = 0;
  let firstInput = num;

  let temp = firstInput;

  if (temp < 10) {
    temp = "0" + temp;
  }

  while (true) {    let a = temp % 10;
    let b = Math.floor(temp / 10);

    answer = String(a) + String((a + b) % 10);
    temp = answer;
    cycle++;

    if (temp == firstInput) {
      break;
    }
  }

  console.log(cycle);
  rl.close();
});
```
