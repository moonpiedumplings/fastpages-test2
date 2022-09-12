---
- toc: true
- title: Making A Quiz In App Lab
- author: moonpie
---

# mMaking a quiz in app lab

```
var questions = ["How many players?"];
var answers  = ["11"];
var boxes = [(["13", "12", "15", "11"])];
var grade = 0;
setText("question", questions[0]);
setText("a0", boxes[0][0]);
setText("a1", boxes[0][1]);
setText("a2", boxes[0][2]);
setText("a3", boxes[0][3]);
onEvent("a0", "click", function( ) {
    if (getText("a0") == answers[0]) {
      console.log("correct");
    }
  });
onEvent("a1", "click", function( ) {
    if (getText("a1") == answers[0]) {
      console.log("correct");
    }
  });
onEvent("a2", "click", function( ) {
    if (getText("a2") == answers[0]) {
      console.log("correct");
    }
  });
onEvent("a3", "click", function( ) {
    if (getText("a3") == answers[0]) {
      console.log("correct");
    }
  });

```

This was a working sample of code. I used this to try to test this, and to design the program, with the ultimate goal of making an theoretically infinite quiz that got questions, answers, and correct answers, from a list. 

However, I later hit a road block. I put the working blocks of code in a for loop, but it did not iterate through. For some reason, the onEvent function does not make the for loop iterate through.

I tried to move the events outside the loop, but those did not iterate through as well. 