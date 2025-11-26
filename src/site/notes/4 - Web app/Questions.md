---
{"dg-publish":true,"permalink":"/4-web-app/questions/"}
---

Class Diagram

![Untitled.jpg|400x533](/img/user/4%20-%20Web%20app/img/Untitled.jpg)
Don't repeat method (and attribute) in child if you're not overriding
If we want a function to be changed when inherited (like *sound()*), we need to make the function abstract. But don't forget, make the class abstract if you have at least one abstract function. If only subset of pet (like cat and dog) need the function (*play()*), we use interfaces. If you implement play() from interface, you should also override it in the classes that take it (otherwise it will turn to abstract). So here, cat is abstract, because it doesn't override play().

So:
- avoid repetition
- method:type parameter:return_type
- public/private

![Untitled-1.jpg|400x711](/img/user/4%20-%20Web%20app/img/Untitled-1.jpg)
> [!success]- Why is this wrong?
> You have to override tune() in StringInstrument because it will turn abstract.
> If instrument wasn't abstract, you wouldhave to override there too 

Playable p = new StringInstrument();

Instrument i = new Instrument; //if abstract → wrong
Instrument i = new StringInstrument; //if abstract → correct


Question s1 = new Question("q1");
Question s2 = new Question("q2");
Question s3 = new Question("q3");
s2 = s1;
s3 = s2;
s1 = new Question("q4");

how many objects will be garbage collected?

> [!success]- Solution
> s1 → q1     (s1=q4 ⇒ s1 garbage collected)
> s2 → q2     (*s2=s1=q2* ⇒ s2 garbage collected)
> s3 → q3     (s3=*s2=s1=q2*)
> 

NaN → if you try to add something, or do operation only related to numbers to something that isn't. What is the type of NaN (number)?

Foreign key unique → 1-1
No constraint on foreign key → many-to-one
Third table to represent (two foreign keys) → many-to-many

I gave them studentTable + coursesTable + enrolTable. 
enrolid = primary key. **What is the relationship between enrolid and course?** 

Question 2 from M1
```html
<!DOCTYPE html>
<html>
	<head></head>
	<body>
		<input type="text" id="input" placeholder="Enter sentence">
		<button id="btn">Rotate</button>
		<ul id="list"></ul>
		
		<script src="midterm.js"></script>
	</body>
</html>
```

```javascript
let btn=document.getElementById("btn"); 
let list=document.getElementById("list");
let flag = false; //have flag to know whether you read input already

let original = "";
let words = [];

function rotate() {
//read input
if(flag==false){
	original = document.getElementById("input").value.trim(); //.value to read value from input   .trim() for whitespace
	words = original.split(" "); //get words into array
	flag=true;
}
//rotate
let first = words.shift();
words.push(first);

let rotated = words.join(" ");
let li = document.createElement("li");
li.textContent=rotated;
list.appendChild(li);

//stop eventListener
if(original==rotated) {
	btn.style.backgroundColor = 'red';
	btn.removeEventListener('click', rotate);
}

}
btn.addEventListener('click', rotate);
```


Ask professor what we need to know from servlets.


See question from other section quiz
