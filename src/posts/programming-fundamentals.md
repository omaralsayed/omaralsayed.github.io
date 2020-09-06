---
title: "Programming Fundamentals"
date: "2019-09-19"
path: "/programming-fundamentals"
author: "Omar"
tags: ["demo", "talk"]
---

On September 2019, I presented the foundations of C++ programming with an interactive demo primarly focused on hyping up the students before MakeUC 2019.

Every Fall semester, we get thousands of new college students, this talk was early in the semester and was primarly targeted toward these students. Most attendees had very basic understanding of programming with no knowledge about how it can be applied in real life.

I explained what an "algorithm" is and how to trace one using a simple trace table. I also reinforced usage of loops in this segment and got live feedback from the audience.

```cpp
int i, x = 0;
for (i = 1; i <= 10; i++) {
    x = i * 2;
}
```
Later on, I went more in depth into loops and presetned an infinite loop example.

```cpp
for( ; ; ) {
    printf("I will keep printing this text forever...unless you stop me.\n");
}
```
Then I gave a consice introduction to the Standard Template Library (STL).

After discussing the basics of loops, code tracing, STL, and running C++ code in the terminal, I jumped into a real-life situation of how they can apply these concepts at a hackathon.

One of the practical uses of C/C++ is Arduino programming and it is one of the topics that the audience gauged interest in via a pre-talk survey, so I discussed some of its concepts.

```cpp
// ledPin is a constant meaning that it will not change
const int ledPin =  LED_BUILTIN; // LED pin number

// ledState is a variable that will change throughout the program
int ledState = LOW;              // Used to set the LED

// "unsigned long" should be used for variables that hold time
// The value will become too large for "int" to store
unsigned long prevMillis = 0;   // Last time LED was updated

// Make interval a constant
const long interval = 1500;     // Blinking interval (milliseconds)

void setup() {
  // Set the digital pin as output
  pinMode(ledPin, OUTPUT);
}

void loop() {
    // Code that needs to be running all the time
}

```

I ended my talk with a live coding demo showing how a simple program can make an LED device blink. This encourged many of the attendees to try out C/C++ at MakeUC 2019.