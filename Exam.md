[1.Emotify the Sentence](https://edabit.com/challenge/Szh3ib2bpJCYXKrKa)

Solution

```js
function emotify(str) {
	if(str == "Make me smile"){
		return "Make me :D"
	}else if(str == "Make me grin"){
		return "Make me :)"
	}else if(str == "Make me sad"){
		return "Make me :("
	}else{
		return "Make me :P"
	}
}
```

[2.Older Than Me](https://edabit.com/challenge/iwdZiFucR5wkQsFHu)

Solution

```js
class Person {
	constructor(name, age) {
		this.name = name
		this.age = age
	}
		
	compareAge(other) {
		let i = Math.sign(other.age - this.age),
				x = ["the same age as", "older than"][i] || "younger than";
		return `${other.name} is ${x} me.`;
	}
}
```

[3.Equality of 3 Values](https://edabit.com/challenge/PKiTjA7SLK99ZZ8GK)

Solution

```js
function equal(a, b, c) {
	if(a == b && a == c){
		return 3
	}else if(a == b || a == c){
		return 2
	}else if(a != b || a != c){
		return 0
	}
}
```

[4.Special Arrays](https://edabit.com/challenge/wikfKaQm3zP7buRA4)

Solution

```js
function isSpecialArray(arr) {
	return arr.every((n, i) => n % 2 === i % 2);
}
```

[5.Explosion Intensity](https://edabit.com/challenge/XnZAcvr4tCD9ppyrN)

Solution

```js
function boomIntensity(n) {
	if (n < 2) return 'boom';
	let boom = `B${'o'.repeat(n)}m`;
	if (!(n % 2)) boom += '!';
	if (!(n % 5)) boom = boom.toUpperCase();
	return boom;
}
```

[6.Basic Arithmetic Operations](https://edabit.com/challenge/mgCKn998CNowjAZBF)

Solution

```js
function operation(a, b, op) {
	if(b == "0" && a != "0"){
		return "undefined"
	}else if(op == "add"){
		return eval(a + "+" +  b)
	}else if(op == "subtract"){
		return a - b
	}else if(op == "divide"){
		return a / b
	}else{
		return a * b
	}
}
```

[7.Common Divisor of Array](https://edabit.com/challenge/rSZmP2dWjEK8Gqcih)

Solution

```js
function gcd(arr) {
	arr = arr.sort((a,b) => a - b);
	let greatest = 1;
	for(let i = 1; i<=arr[0]; i++){
		if(arr.every(num => num % i === 0)) greatest = i;
	};
	return greatest;
}
```

[8.Largest Swap](https://edabit.com/challenge/hD3euqPHM82Cbr7R8)

Solution

```js
function largestSwap(num) {
	return num / 10 > num % 10
}
```
