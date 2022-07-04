---
layout: post
title:  "How I Taught Python in TEJ4M"
date:   2021-08-09 15:01:43 -0400
page.categories: resources
feature_image: https://images.unsplash.com/photo-1508780709619-79562169bc64?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1050&q=80
---

One of the great things about the TEJ (Computer Engineering) curriculum is that its expectations can be covered in multiple ways. It can be tailored to student needs and interests, as well as the strengths of the individual teacher teaching the course.

My educational background is in computer science, so I tend to place a tad more emphasis on the coding expectations that are included in the 
curriculum:

{% include figure.html image="/assets/B5expectations.PNG" alt="Screenshot of the TEJ4M B5 curriculum expectations" position="center" %}

In TEJ4M this past year, I taught two different languages: Python and Arduino. Working with the Arduino is nice because it hits a lot of the other expectations as well that have to do with interfacing, circuitry, and robotics. Python not only covers the specific expectations highlighted above, but it can also be loosely tied to other expectations that have to do with careers and post-secondary education. As part of our unit of study, we looked at open source software and how to use industry tools like Github.

Python is widely considered to be an easy and beginner-friendly language to learn. Its syntax is much more simplistic than Arduino's C++, which is nice for students who have never coded before. It's also very popular, [recently surpassing Java](https://redmonk.com/rstephens/2021/08/05/top-20-june-2021/). It's a language that I want my students to at least have a basic understanding of, as the field of Computer Engineering grows to include programming and software skills as well as hardware skills.

#### What I Want My Students To Know & Be Able To Do

I covered the basics of Python up to functions. I taught all of the usual concepts of the language:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Variables, Data Types, Strings, and Lists

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Conditionals

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Loops

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Basic Functions

Partially due to the quadmester format, and also because this is __not__ a computer science (ICS course code) class, we didn't cover these topics in a ton of depth- for example, string slicing and dicing was not covered, nor dictionaries. But these four concepts are enough to be able to do some pretty neat things with the language and develop a good foundation.

In terms of assessment, each of those concepts formed the basis of what I called __Knowledge Checks__, small programming questions (1-5) that weren't intended to take more than an hour to complete. I tried to stress the importance of __process over correctness__ and __concepts over syntax__ with these assessments, since they were supposed to be formative in nature. I wanted to see how my students were grasping each concept and whether or not they could apply it. Because I was teaching online, the results were a tad dubious at times. If I was to replicate this in person, I think I'd actually get my students to submit their answers on paper and in class, without the use of computers. This does two things:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. It checks for true understanding of the concept, since students can't use computers to check their code for correctness

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Post-secondary institutions will sometimes assess code written on paper, and this prepares students for that in a very low-stakes way

Once we had covered the basics of the actual language, I used Python as a springboard into other topics. Python has a very strong open source community. I had my students do a small research assignment on the different open-source libraries that Python offers and brainstorm ideas or find examples for how they may be used in the software industry, and present their findings in the form of a creative poster. This let students explore their personal interests a little more, but it also gave them a glimpse at how the language might also be useful to them in the future. Their research had potential ties to other areas of the curriculum as well: Python has libraries for networking, robotics, and machine learning.

Python also has a built-in library called [_dis_](https://docs.python.org/3/library/dis.html), which disassembles Python bytecode. Using this library we were able to explore how Python _actually_ works and what makes the language so portable, and it led us to a discussion about various low-level languages. At this point my students had already been coding in Python, so we were able to compare code that was previously written in class to its disassembled, low-level equivalent.

{% include figure.html image="/assets/pythondis.PNG" alt="Screenshot of a comparison between Python code and its disassembled bytecode." position="center" caption="A very simple Python function on the left, and the output of running dis.dis(isEven) on the right." %}

When I first learned assembly in university, one of the assignments we were given was to examine a piece of ARM assembly code and translate it back to its C equivalent. I replicated a similar version of this assignment for my Grade 12s, but with Python instead. After introducing them to the _dis_ library, I gave them a set of disassembled bytecode to reverse engineer, first by annotating the output to identify what each block did, then combining these notes into complete high-level Python code.

#### Next Steps & Final Thoughts

Over the past school year, I began to experiment with [CircuitPython](https://circuitpython.org/). It's based on Python, but I think it could also potentially replace Arduino and be used to cover all of the same expectations. This simplifies the teaching a bit- students would only have to learn Python syntax. I picked up a [starter kit](https://www.adafruit.com/product/4028), soldered the header pins on, updated the firmware, and it worked! (Honestly, this process could be a blog post on its own...)

{% include figure.html image="/assets/blinkingled.gif" alt="Blinking red LED powered by CircuitPython and ItsyBitsy M4 Express microcontroller" position="center" caption="It works!!! This is the ItsyBitsy M4 Express by Adafruit." %}

I've also heard interesting things about Raspberry Pi Pico, but I haven't looked much into that yet!

Either way, teaching Python was one of my favourite units in this course. There are so many potential applications and curriculum connections aside from just coding. For me personally, I want to experiment more with CircuitPython and learn more about the Raspberry Pi Pico as possible replacements for teaching Arduino. 