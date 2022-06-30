
1. var의 경우 변수선언에 있어서 혼란의 부분이 존재

ex) var age = 10;
console.log(age); // 10

var age = 20;
console.log(age); //20

* 이경우 정상출력 되면 안됨. 변수를 한번 더 선언했기 때문
기존변수에 새로 작성한 변수가 덮어씌어지는 문제 발생

let age = 10;
console.log(age); // 10

let age = 20; // error
* let의 경우 이미 선언한 변수에 값을 다시 할당할 수 있음.

let age = 10;
age = 20;
age = 30;

---
**var**의 경우 블록스코프 {..}를 가지지 않기떄문에 블록 밖에서 접근이 가능
**let**의 경우 밖에서 접근하면 에러가 발생함.

{
	let age = 10;
}
console.log(age); // error

{
	var age = 10;
}
console.log(age); // 10

