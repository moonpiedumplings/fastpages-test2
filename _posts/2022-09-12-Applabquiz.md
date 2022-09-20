---
- title: Making A Quiz In App Lab
- toc: true
- author: moonpie
---

# Making a quiz in app lab

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

The variables (lists) I used are an example of data abstraction. My goal was to create multiple lists that can be fed to the program. 

However, I later hit a road block. I put the working blocks of code in a for loop, but it did not iterate through. For some reason, the onEvent function does not make the for loop iterate through.

I tried to move the events outside the loop, but those did not iterate through as well. 

I'm going to redesign this with a while loop, that changes after onEvent is clicked. 


However, this was too tedious. I collapsed this down into a function.

```
function checkAnswer(b) {
  if (getText(b) == answers[i]) {
      console.log("correct");
      grade++;
      i++;
    }
    else {
      console.log("incorrect");
      i++;
    }
  setQuestions();```

  The setQuestions function does exactly that, set questions according to the list,using the variable i pick from the lists. Whenever a button is clicked, this function is called and the answer is checked, the variable grade is changed, and the new questions are set. This is an example of procedural abstraction. The question setting is one function, and the answer checking is another. 