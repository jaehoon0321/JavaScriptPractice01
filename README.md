# JavaScriptPractice01

## 변수

**1.** 다음 중 재할당이 불가능한 선언은?

A) `var a = 1`  B) `let a = 1`  C) `const a = 1`

정답 : 3번 

var a = 1 -> 1을 a에 담겠다 
let a = 1 -> 1을 a에 담겠따 

**2.** 아래 코드의 출력결과는?

console.log(x);
var x = 10;

정답 -> x라는 변수에 10을 지정하겠다 x=10

**3.** 아래 코드에서 에러가 나는 줄은? 이유는? 

```jsx
1 console.log(y);
2 let y = 3;
```
정답 -> 1번줄 
이유 -> 호이스팅 : 변수나 함수를 스코프 상단으로 끌어올리는 것으로 버그의 원인이다.

**4.** `const obj = { n: 1 };`   

    obj 객체의 속성 n 의 값을 2로 변경하세요.


정답 :Sol1)-> 점표기법  obj.n=2;  Sol2)대괄호 표기법 -> obj['n']=2;


  **5.** 다음 중 올바른 식별자(변수명)가 아닌 것은?

A) `_count` B) `$value` C) `2nd` D) `camelCase`

정답 : B

-> A. "_" 밑줄은 식별자의 시작 문자로 허용
-> B. $ 기호도 시작 문자로 허용 


**6.** 다음 코드의 결과?

```jsx
let a = 1;  a라는 변수에 1을 담는다 
a = a + 2;   a= a+2 -> a= 1+2
console.log(a);  a를 출력해라
```
정답 a = 3
---

# 문자열

**7.** 템플릿 리터럴로 “Hello, JS!”를 만들 올바른 코드는?

A) `'Hello, ${"JS"}!'` B) ``Hello, ${"JS"}!`` C) `"Hello, ${"JS"}!"`

정답 : B

템플릿 리터럴이란? 개념 공부

템플릿 리터럴은 2015년에 도입된 ES6표준에 포함된 기능 이전에 일반 문자열(''나 ""보다) 더 유연하게 쓸 수 있음 

1.백틱
 ($\texttt{\`}$) 사용

 EX) 
 const name = "jaehoon";
 const mg = "Hello" + name(jaehoon) + "i'm javaScript";

 -> 백틱을 사용하게 된다면?

 const mg = `Hello ${name}!`; 코드를 더 간결하게 사용 가능 
 
 


**8.** `"abc".length` 값은?

정답 : 3

<lengh 개념공부>
length 문자열의 길이를 나타냄 abc -> 문자열 3 




**9.** `"Hello".toLowerCase()` 결과는?

<.toLowerCase 메서드 개념공부>
Lower 소문자
모든 영문 대문자를 소문자로 

정답 hello



**10.** `"  hi  ".trim()` 결과는?

<trim 메서드>
문자열 양 끝에 있는 공백을 제거해준다

정답 :양쪽 공백없는 hi


**11.** `"a,b,c".split(",")` 결과는?

<.split 개념공부>
특정 구분자를 기준으로 문자열을 나눈다
split 을 ","기준으로 나누기 때문에 


정답 : "a","b","C"


**12.** `"abc".includes("b")` 는 `true`?

<.includes 개념공부>
.includes 는 해당하는 문자가 포함이 되어있으면 ture 아니면 false를 반환한다 , 대소문자 구분함.

정답 : ture



**13.** `"cat".replace("c","b")` 결과는?

c를 b로 바꿔.

정답 : bat


조건문 
14. 아래 출력결과는?
console.log(2 == "2", 2 === "2");

2와 같아? "2" TRUE
2와 같고 type 일치해? true, false

== 동등연산자(값만 비교)
===일치 연산자(값과 타입 비교)
2==="2" 를 만족시키려면 Number, parseInt를 사용하여 문자타입을 숫자 타입으로 바꿔줘야함. 

정답 : true false

​
15. 삼항연산자 결과는?
const n = 5;
const r = n % 2 === 0 ? "even" : "odd";

<삼항연산자 개념공부>
n=5
5/2=(나머지 1)이 출력
5를 2로 나는 나머지의 값이 0과 일치하느냐 (===) 일치연산자 ->? 조건식의 끝을 알려주고 -> 참이면 even을 거짓이면 odd를


정답 : odd


​
16. switch 기본형에서 일치 비교에 쓰이는 것은?
A) ==  B) ===  C) 둘 다

정답 B




17. && 단축 평가 결과:
    
const ok = true && "DONE";


&& AND 연산자 

정답 DONE



18. 속성 접근 결과?
const user = { name: "Ann", age: 17 };
console.log(user["name"]);

user 안에 name속성에는 ann age라는 속성에는 17
출력해라 user name을 Ann

정답:Ann


​
20. 키를 추가한 다음 코드의 결과는?
const k = "score";
const obj = {};
obj[k] = 100;
console.log(obj.score);

k 에 score을 넣어주고 
obj 에 빈객체 넣어주고 
obj[k]에 100을 넣어주고
출력해라 

정답 : 100



21. 다음의 출력결과는?
    
const a = { n: 1 };
const b = { n: 1 };
console.log(a === b);

{} 객체 리터럴이고 
{ n: 1 }이건 n:1을 담고이는 객체 그 자체 
a와 b가 같아? 일치 연산자 일치하면 ture 일치하지 않으면 false

정답 a = b변수의 객체들이 일치하므로 true





Array (배열~)

21. const arr = [1,2,3]; arr.push(4); 이후 arr는?

push -> 넣다 pop-> 마지막 입력 요소 버림/반환 (기본 배열은 0부터 시작)


정답 :1,2,3,4


22. pop()이 반환하는 것은?

정답 : 4


23. slice(1,3)의 의미와 arr에 적용한 결과는?

    slice= 배열의 일부를 복사하여 새로운 배열에 적용하는것

  값이 12345
  인덱스는 01234

  slice 1 3 을 하면 
  인덱스의 1 3값 
  234를 들고오는거고
  출력은 2,3 이게 아닌가.

  24.splice(1,2)의 의미와 arr에 적용한 결과는?

  .splice(1,2)메서드 
  배열을 직접 수정하며  요소를 제거 

  인덱스 1부터 시작을 하고 
  시작 인덱스로 부터 2개를 제거한다.

   ex)
   인덱스는 배열이기 때문에 0,1,2,3,4
   값은 1,2,3,4,5 라고 치면

   .splice(1,2)
    인덱스 기준 1에서 시작해서 2개를 제거한다. .

    
25. map 결과?
[1,2,3].map(x => x * 2)

<개념공부>
map() 메서드  -> 배열의 각 요소에 대해 주어진 함수를 실행,
반환값을 모아서 새로운 배열을 만들어 반환

x에 1, 2 , 3 따로 따로  
2,4,6



26. filter 결과?
[1,2,3,4].filter(x => x % 2 === 0)

<개념공부>
filter()메서드는 말그대로 필터 조건에 맞는 값만 통과시키고 새로운 배열로 반환해줌

x를 2를 나눈것 0과 일치하면 반환
 === 일치연산자(두 가지 조건을 만족해야지만 반환해줌)

 


27. includes 사용한 결과는?
[1,2,3].includes(2)

<개념 공부 > includes는 영단어 그대로 포함한다는 의미
[]이건 배열이고  안에 배열 값 1,2,3

배열안에 2가 포함되어 있니?


정답: True


28. reduce 결과는?
[1,2,3].reduce((acc, cur) => acc + cur, 0)

<알아야될 개념>
acc (누산기를 의미)
이전단계까지 계산결과가 누적

reduce() 메서드 공부 `
arr.reduce((누산기, 현재_값) => 계산식, 초기_값)

[1,2,3].reduce(acc,cur)-> acc + cur, 0


Loop 반복 

29. for (let i=0; i<3; i++) console.log(i); 출력?

<개념>
for 반복문

let,var

i=0부터 시작해서 3미만 까지 ++ 증감 연산산자

정답 0 1 2 


30. for...of는 어떤 것을 순회할때 효과적인가?

for...of 반복 가능한 객체(Iterable Objects), 메서드를 가지고 있어 요소들을 하나씩 순서대로 꺼낼 수 있음.

배열 문자열처럼 순서가 있는 데이터의 값을 하나씩 처리할때 가장 효과적

31. for...in은 주로 무엇을 순회할때 효과적인가?

    속성 이름을 순서대로 반복 할때 효과적이다.

32. 다음 코드의 마지막 sum의 결과값은?
let i=1, sum=0;
while(i<=3){ sum+=i; i++; }

let i=1 을 지정해주고 sum = 0 으로 초기화
while 반복문 i 가 3이하까지 
1 ,2,3 =6

정답 6

33. for...of 출력 결과는?
for (const ch of "Hi") console.log(ch);

정답:
H
i

개념: for of  문 반복 가능한 객체 각 요소 값을 순서대로 순회.


34. 빈칸에 들어갈 키워드는 무었인가? 
const arr = [10, 20, 30];
for (const num ___ arr) {
  console.log(num);
}

정답 ->  of

const 불변 지정을 해주고 10,20,30

for of 을 사용 해서 값을 순회할때 사용하는 반복문



35.아래 colors 배열의 요소값을 순서대로 출력하는 반복문을작성하세요 
const colors = ["red", "green", "blue"];


정답: red , green, blue 
const colors = ["red", "green"," blue"];

for (const color of colors) {
    console.log(color);
}


36.아래  str의 요소를 순회하여 출력하는 반복문을 작성하세요.
const str = "JS";

for (const char of str){
    console.log(char);
}

37.  배열 scores의 점수에 대한  총점과 평균을 구하여 출력하는 코드를 작성하세요.
const scores = [90, 80, 70];

불변 scores = 배열지정 90,80,70

const totalSum = scores.reduce((acc.cur) => acc + cur, 0)

-totalSum => sores.re

const average = totalSum / scores.length;


reduce 배열 요소들의 총합을 계산할때 사용하고 , 객체 변환 , 배열의 쵀대/최소값을 찾을때도 쓰긴함.
화살표 함수 =>
(매개변수) => { 함수 본문(실행할 코드) }

39. user 객체의 정보를 출력하는 반복문을 작성하세요.
const user = { name: "Yumi", age: 20 };

객체의 정보를 반복을 해야 하니 for in을 써야 함

 for(const key in user);{
     console.log(key);

40.arr 배열의 요소값을 forEach문을 이용하여 출력하세요. 
const arr = [1, 2, 3];

arr.forEach(e=>{
    console.log(e);
    });
     
**41.** `Map 이란`?
Map 객체는 키와 값을 한 쌍으로 이루어진 컬렉션
prototype? map 객체 안에는 프로토 타입이 있는데 안에서 set라는 메소드를 통해 저장할 수 있다. 

map이라는 객체를 클로닝  원형에서 제공하는 속성들이 있을거임 이것이 프로토 타입 기능들을 보여주고 있음 

자가복제 느낌으로 알아두면 좋음.

생성
const map = new Map();



**42.** `Set`이란?
 내장 객체, 중복을 허용하지 않는 유일한 값들의 집합을 저장 할때 사용

 43. 아래 Map의 결과는? 
const m = new Map();  -m 이라는 새로운 map객체 생성
const k = {}; -> k라는 새로운 빈 객체를 생성->( 메모리 주소를 가진 객체 ) 
m.set(k, 123); -> m.set set메서드를 이용 Key는 k이고 값은 123
console.log(m.get(k));\





 
```jsx

```

**44.** 아래`Set의 결과는?`

```jsx
const s = new Set([1,2,2,3]);
s.add(3);
console.log(s.size);
```
불변 s로 지정 새로운 Set을 지정 중복된 값 제거 2가 중복 됐으므로 
1,2,3
s에 add. 3의 값을 추가하려 하는데 3 이 있고 중복은 불가 하므로 

결과 1,2,3

**45.** `Map` 크기 확인 프로퍼티는?

정답 : size


