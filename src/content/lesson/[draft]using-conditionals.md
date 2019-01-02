---
subtitle: "There is now way you can throw 3 lines of code in an algorithm without have to include a conditional. It's time to guide the computer on how to make decisions!"
status: "draft"
title: "Using Conditionals in Coding"
cover: "https://ucarecdn.com/4cc6fa0b-2530-4052-aa7e-8dac03788ac3/"
textColor: "white"
date: "2018-12-12"
tags: ["conditional rendering", "if else", "using conditionals"]

---

## What is a condition?

We make decisions every day since we wake up, most of them are already automated in our brains like taking a shower and some other requiere more attention like were to invest money or deciding were to eat with your partner :smile:.

A very similar process can happen when coding, you can create scripts (algorithms) that automate the computer behavior and decisions depending on certain conditions.

## What is a condition?

A condition is just something that needs to happen before something else can happen. For example: A baby monitor that sends you an SMS when... the sound or camera signal variations occur.

In coding, to tell the computer how to make a decision based on a condition you use the word: `IF`

`If`... 
**signal is detected on the mic or camera**... 
send an sms to +1345 5557777.

`ELSE`... do nothing.

If programing terms, a condition its a wat to limits the execution of a particular block of code depending on one or more variable having expected values.

## How to code a condition

If you are using Javascript conditions can be coded using the `if... else` syntax, for example asuming you have a variable called `babyHasMoved` that you know it will always contain a boolean inside (that can be either true or false), you could have the following condition:
```js
if(babyHasMoved === true){
	sendSMS("The baby has moved just now", +13455557777)
}
```  
[[warning]]
| :point_up: Notice how we are using 3 equal symbols instead of just one. That is because we are asking a question to the computer, if we use just one equal the computar will think that we are assigning the value `true` to the variable `babyHasMoved`. It is called a [logical operation](https://www.youtube.com/watch?v=mbT7sSmVUS8).

You could have a block of code execute only if the condition does not apply using the `else` statement:
```js
if(babyHasMoved === true){
	sendSMS("The baby has moved just now", +13455557777);
}
else{
	//this will only execute if babyHasMoved is different than true 
	sendSMS("The baby has NOT moved", +13455557777);
}
``` 

Or you could have separate conditionals asking in different ways:
```js
if(babyHasMoved === true){
	sendSMS("The baby has moved just now", +13455557777);
}
if(babyHasMoved === false){
	sendSMS("The baby has NOT moved", +13455557777);
}
```

## Combining different logical operations

Some times the situation is more complicated and you need several variables to be able to ask the right question, for example: Should I wear the blue shirt today? Only if it is not dirty, if it fits me and also if the color matches with the pant.

#### The `AND` operator:

Those are 3 separate questions that you can ask on the same condition using **the AND operator** that in Javascript is represented with two amperson characters `&`:

```js
let isDirty = true;
let shirtColor = "blue";
let size = "M";

if(isDirty === false && shiftColor == "blue" && size == "M"){
	putOnShirt();
}
```

#### The `OR` operator:

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDgyMTUzNzQ0LC0yMjEwOTI1OTcsLTEwMD
MyNzUzODAsLTY4OTMzMDI3NCwyMDk4ODY3Mjc4LDEyMzg2OTAx
NDYsLTE2MzUwNDcyOTMsLTEyMjcyNjYzNzAsNzMwOTk4MTE2XX
0=
-->