# Natalie Ti's User Page

---

## Table of Contents

1. [About Me](#about-me)
2. [Skills & Tools](#skills--tools)
3. [How I work](#how-i-work)
4. [Hobbies and interests](#hobbies-and-interests)
5. [Really cool code](#really-cool-code)

---

## About Me

Hello! I'm **Natalie Ti**, a third-year Cognitive Science Design/Interaction major minoring in Computer Science. I like doing website design and frontend coding.

---

## Skills & Tools

### Programming languages (ranked)
1. **JavaScript and HTML/CSS**
    - React and Node.js
    - MantineUI (so cool the documentation is so helpful)
2. **Python** 
3. **C**
4. **Java**
5. **C++**

### Other tools
- Figma 
- Adobe Creative Suite 

### Some goals I have 
- [ ] Try using particles.js for particle effects on web pages
- [ ] Use three.js to make an interactive 3d element


---

## How I work

I tend to work in **sprints** and have a habit of scratching everything and starting anew. I like to **modularize** my work so that parts can be reused or aren’t hyperspecific to a single page (like widget styles).

Sometimes I ~~procrastinate~~ so I suppose I should

> "Start early and start often."  
> — *every CS professor at UCSD*

I like JavaScript and all but the one thing I can't really get used to is the function shortcut notation:
`const add = (a, b) => a + b;` The lack of brackets confuses me sometimes.

---

## Hobbies and interests

Some of my hobbies include:

- **Hair Styling:** cutting, bleaching, and dying hair 
- **Cooking:** i'm a big fan of pasta    
- **Sewing:** i have a thing for dolls

One of my favorite things to do is listen to music on the bus. My current favorite song is [**Death & Romance** by Magdalena Bay](https://youtu.be/xMJyxP-kUWg?si=pRaNMMsRImHG452q).

---

## Really cool code

This cat can be drawn using this code for HTML5 Canvas:

[Cat Image](beautiful%20cat.png)

```javascript
const canvas = document.getElementById("catCanvas");
const ctx = canvas.getContext("2d");

ctx.strokeStyle = "black";
ctx.lineWidth = 2;
ctx.fillStyle = "black";

const headX = 100;
const headY = 150;
const headRadius = 20;
ctx.beginPath();
ctx.arc(headX, headY, headRadius, 0, Math.PI * 2);
ctx.stroke();

//ears
ctx.beginPath();
ctx.moveTo(headX - 15, headY - 10);
ctx.lineTo(headX - 25, headY - 30);
ctx.lineTo(headX - 5, headY - 15);
ctx.closePath();
ctx.stroke();

ctx.beginPath();
ctx.moveTo(headX + 15, headY - 10);
ctx.lineTo(headX + 25, headY - 30);
ctx.lineTo(headX + 5, headY - 15);
ctx.closePath();
ctx.stroke();

//eyes
ctx.beginPath();
ctx.arc(headX - 7, headY - 5, 2, 0, Math.PI * 2);
ctx.fill();
ctx.beginPath();
ctx.arc(headX + 7, headY - 5, 2, 0, Math.PI * 2);
ctx.fill();

//nose
ctx.beginPath();
ctx.arc(headX, headY + 2, 2, 0, Math.PI * 2);
ctx.fill();

const neckX = headX + headRadius;
const neckY = headY;
const bodyEndX = 220;
ctx.beginPath();
ctx.moveTo(neckX, neckY);
ctx.lineTo(bodyEndX, neckY);
ctx.stroke();

//front legs
ctx.beginPath();
ctx.moveTo(neckX + 5, neckY);
ctx.lineTo(neckX + 5, neckY + 30);
ctx.stroke();

ctx.beginPath();
ctx.moveTo(neckX - 5, neckY + 15);
ctx.lineTo(neckX - 5, neckY + 30);
ctx.stroke();

//back legs
ctx.beginPath();
ctx.moveTo(bodyEndX - 5, neckY);
ctx.lineTo(bodyEndX - 5, neckY + 30);
ctx.stroke();

ctx.beginPath();
ctx.moveTo(bodyEndX + 5, neckY);
ctx.lineTo(bodyEndX + 5, neckY + 30);
ctx.stroke();

//tail
ctx.beginPath();
ctx.moveTo(bodyEndX, neckY);
ctx.quadraticCurveTo(bodyEndX + 30, neckY - 20, bodyEndX + 20, neckY + 10);
ctx.stroke();

```
