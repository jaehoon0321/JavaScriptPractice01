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
  출력은 2,3 이게 아닌거.
  다시공부.  


  


26. splice(1,2)의 의미와 arr에 적용한 결과는?






27. map 결과?
[1,2,3].map(x => x * 2)
​
28. filter 결과?
[1,2,3,4].filter(x => x % 2 === 0)

29. includes 사용한 결과는?
[1,2,3].includes(2)
​
30. reduce 결과는?
[1,2,3].reduce((acc, cur) => acc + cur, 0)
​
Loop 
31. for (let i=0; i<3; i++) console.log(i); 출력?
32. for...of는 어떤 것을 순회할때 효과적인가?
33. for...in은 주로 무엇을 순회할때 효과적인가?
34. 다음 코드의 마지막 sum의 결과값은?
let i=1, sum=0;
while(i<=3){ sum+=i; i++; }
35. for...of 출력 결과는?
for (const ch of "Hi") console.log(ch);
​

36. 빈칸에 들어갈 키워드는 무었인가? 
const arr = [10, 20, 30];
for (const num ___ arr) {
  console.log(num);
}


​
35.아래 colors 배열의 요소값을 순서대로 출력하는 반복문을작성하세요 
const colors = ["red", "green", "blue"];


```jsx

```

1. 아래  str의 요소를 순회하여 출력하는 반복문을 작성하세요.

```jsx
const str = "JS";
```

37.  배열 scores의 점수에 대한  총점과 평균을 구하여 출력하는 코드를 작성하세요.

```jsx
const scores = [90, 80, 70];
```

---

1. 배열 nums 의 요소값 출력을 2번째 인덱스의 값까지만 출력하는 코드를 작성하세요

```jsx
const nums = [1, 2, 3];
```

39. user 객체의 정보를 출력하는 반복문을 작성하세요.

```jsx
const user = { name: "Yumi", age: 20 }; 
```
40. arr 배열의 요소값을 forEach문을 이용하여 출력하세요. 
const arr = [1, 2, 3];
​
41. Map 이란?
42. Set이란?
43. 아래 Map의 결과는? 
const m = new Map();
const k = {};
m.set(k, 123);
console.log(m.get(k));
​
44. 아래Set의 결과는?
const s = new Set([1,2,2,3]);
s.add(3);
console.log(s.size);

45. Map 크기 확인 프로퍼티는?
