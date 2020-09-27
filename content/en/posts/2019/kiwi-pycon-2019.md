---
title: "Microscopic Summary About My First Pycon"
date: 2019-08-27T04:48:57+13:00
description:
url: /kiwi-pycon-2019/
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: inner
tocLevels: ["h2", "h3", "h4"]
tags:
- Data Science
- Technology

series:
- 
categories:
- Data Science
- Technology
image: /images/2019/pycon.jpg
---
![tut](/images/2019/pycon.png)

<p style='text-align: justify;'>
I attend my first Python conference last weekend. It was the NZ python user group’s tenth national python conference. Everything was just great and awesome; I made a lot of friends also learn a lot. Going to a conference full of people who love the same thing as myself is always a fun experience. There’s so much more to PyCon than just a bunch of people talking about the Python language. Everyone who attends PyCon may have a different experience, and that’s what makes the conference truly unique right!</p>

<p style='text-align: justify;'>
Here is a microscopic summary of the talks I picked. I tried to summerise the talk, linked to the YouTube videos and GitHub accounts to one post what wiser ones speak at the conference. I would share some of the notes that I’ve taken over the conference to help you get the most out of my PyCon experience in a future post.</p>

## 1. A Beginners Intro to the Flask Web Framework from Steve Dunford

<p style='text-align: justify;'>
In my opinion, the flask is probably the best web framework out there and we should consider learning and using it in 2019. Flask is perfect for beginners that want to get started as quickly as possible and also for a more experienced developer who craves freedom and flexibility. Steve went over how to make a simple data-backed website with Python. He covered how to combine Flask, SQLite, HTML, CSS, and some common flask add-ons to make a very simple version of IMDB. Here is the <a href="[url](https://repl.it/@chadz009)">code snippet</a> I practiced and the <a href="[url](https://drive.google.com/file/d/1ZGDgBF7PtVJ8oe84c6g66k5V6UfvSpg2/view)">Pdf version</a> of the Tutorial.<p style="color:#13d1c4";>NOTE: All credit to Steve Dunford giving permission to share the tutorial.</p> </p>

## 2. Python Debugging: Pro Tips and Not-So-Obvious by Dave Glover

<p style='text-align: justify;'>
Following Dave’s tutorials was great. I got exposure to new skills and made me crave dig more into Python in the cloud. Also, debugging tips are massive eye-opener too. Basically, in the first half, he talked about debugging remote python in environments such as Circuit Python, Raspberry Pi, Docker containers, remote Linux Servers, and Jupyter Notebooks. Then went over how to sync code to devices, attach debuggers, and step through code.</p>


![tut](/images/2019/tut-time.png)

>  It’s the tutorial time!

<p style='text-align: justify;'>
Second half he went through how to configure Visual Studio Code to be a powerful and productive development environment that enables us to quickly and easily create and debug Python apps and how to develop scalable web applications using Django and PostgreSQL, and deploy them to the cloud on Azure in just a few clicks.Here is Dave’s <a href="[url](https://github.com/gloveboxes/PyCon-Hands-on-Lab)">Git hub account</a>  where he shares both of the labs.</p>

## 3. The Natural State of Computers by Amber Brown

<p style='text-align: justify;'>
Asynchronous programming has been gaining a lot of attention in the past few years, and for good reason. Although it can be more difficult than the traditional linear style, it is also much more efficient. Amber Brown, a core developer and release manager from a twisted asynchronous networking library went over how does this Asynchronous programming solve the problems. During her talk, she investigates that the common tasks that we as a developer implement, we can find which ones are made easier with asynchronous techniques, and which ones are made more difficult. Check here for Amber’s talk.</p>

{{< alert theme="warning" >}}
Async isn’t just nice. It’s essential. What is driving for a good Async story? I think the reason is computers are simply not getting faster. we have to be more efficient. Lot of networking based workloads, asynchronous I/O is far more efficient than traditional blocking regime"
<cite> - Amber Brown </cite>
{{< /alert >}}

## 4. Python product dev tools for electronics by Barrie Duncan

<p style='text-align: justify;'>
Product developers spend a lot of time interacting with various tools which are vital to the development phase. Whether it’s software, a mobile app, or hardware we are developing, these tools are critical to the success of our project. During the Barrie Duncan’s talk, he went over how the Python Numba package had been key to developing a simulator of new motor technology they invented. Basically, Numba allows them to optimize a lot of code into c code. Rather than write a program specific to the problem, he picked instead to write a general-purpose, although simple, code generator tool. It solved the problem of managing small chunks of generator code sprinkled throughout a large collection of files. Then use this general-purpose tool to solve a specific generation problem was one of his approaches to solving problems we face in the development environment.</p>

![barry-duncan](/images/2019/barry-duncan.png)

> Barrie Duncan about to start his presentation

<p style='text-align: justify;'>
Also, check how he describes how Jenkins helped them create an automation test system for helping to validate their product development and how Jenkins offers a simple way to set up continuous integration and continuous delivery environment for almost any combination of languages and source code repositories. Check what Barrie share here at the conference.</p>

## 5. How to Write Python Code Others Like to Use by Anna Tisch

<p style='text-align: justify;'>
In the last decade, SDK usage has become a major part of the development lifecycle. In fact, it is so commonly used and integrated into products, that one would say developers need to acquire more knowledge with many frameworks rather than learning deep algorithms to implement by themselves. Anna Tisch from Microsoft mainly addressed those who want to learn how to write the best SDK and supply documentation for it. The goal/orientation of an SDK is that its documentation should be focused and clear. Throughout her talk, she went over various best practices we wanted to follow. Check here what Anna share at the conference.</p>

## 6. Getting started with MicroPython on a microcontroller from Glenn Ramsey

<p style='text-align: justify;'>
MicroPython is a subset of the Python 3 language that has been pared down to run efficiently on several microcontrollers. If we are familiar with Python or looking for a quick way to write code for a microcontroller (that isn’t C/C++, Arduino, or assembly), Micro Python is a good option. During Glenn’s talk, he talks/ demonstrated live about getting MicroPython installed on an ESP32 development and how to create a sound meter with visual output. Trust me!! this is a nice fun project to do on one nice weekend while sipping a beer!! Check here what Glenn share at the conference.</p>

## 7. Building an interactive training environment using JupyterHub” from Graham Dumpleton

<p style='text-align: justify;'>
Before Graham Dumpleton’s talk, I didn’t know that we can use JupyterHub to spawn applications other than Jupyter notebooks In this talk he walked through what JupyterHub is and how it works. Also, guide us on how JupyterHub was used to implement a multi-user workshop environment running in Kubernetes. Basically, Instead of creating Jupyter notebooks, JupyterHub was used to create user environments in Kubernetes which gave the user access to an interactive Linux shell environment in their web browser, along with workshop course notes and presenter slides, in the same integrated dashboard view. Because the user environment provided all the tools required for the workshop, users were immediately good to go, with no need to install anything locally on their own computer. Check here How Graham share his expertise at the conference</p>

## 8. Automate Your Integration Tests Using pytest-docker-compose from Phoenix Zerin
<p style='text-align: justify;'>
Docker containers opened a world of possibilities for the tech community, hassles in setting up new software were decreased unlike old times when a mess was to be sorted by a grievous format, it reduced the time to set up and use new software which eventually played a big part for techies to learn new things, roll it out in a container and scrap it when done. Things became easy, and the best thing its open-source anyone, and everyone can use it, comes with a little learning curve though. The possibility of defining a complex stack in a file and running it with a single command, pretty tempting huh! The guys at Docker Inc. choose to call it Docker compose. Check here what Phoenix wants to teach us how to automate our integration testing using pytest Docker compose. Learned a lot!! Wort a check his talk!</p>

{{< alert theme="warning" >}}
Sometimes unit tests aren't enough, and we need to actually deploy our solution to see how it behaves as a whole. Utilities like docker-compose make it easy to stand up an entire environment, but the actual testing part still has to be done manually... or does it? “
<cite> -Phoenix Zerin </cite>
{{< /alert >}}

## 9. From NASA to Startups to Big Commerce by Daniel Roy Greenfeld

<p style='text-align: justify;'>
Daniel Roy Greenfield’s talk was inspirational as well as very informative. Daniel is the Vice President at BriteCore, Co-author of the Two Scoops of Django also Creator of numerous large open-source projects such as Cookiecutter Django. His talk was all about how important it is to focus on the moment instead of always thinking and planning ahead (something I’m guilty of).</p>

{{< alert theme="warning" >}}
 KISS: keep it simple, stupid.
 <cite> Kelly Johnson </cite>
 {{< /alert >}}

<p style='text-align: justify;'>
So what should Daniel tell us about KISS? It really just means we have to keep it simple. Simple code is less prone to bugs and is easier to read and understand for us and the people who’ll be working on the code in the future (including ourselves). And now you’re probably thinking you’re already doing that. Duh, why would you write complex code? Maybe you even think of yourself as not being a good enough programmer to write complex code! See his talk here…</p>

## 10. Turning ‘wat’ into ‘why’ by Katie McLaughlin

<p style='text-align: justify;'>
There many different programming languages. Yes, it is true that we can create a website using Ruby, Java, Python, C#, Go, or JavaScript. You can use C or C++ or Haskell or Rust. Or COBOL or Pascal or Perl. Underlying this fact is that all of these languages serve the same purpose: to turn human thoughts into the 1’s and 0’s that the computer understands. In highfalutin computer terms, they are all “Turing complete”. At their most foundational level, these languages are all the same. But on the surface. where humans interact with them vary a lot.
In this talk, Katie takes us a tour of a dozen different programming languages, from JavaScript to Haskell, Python to Perl, Elixir and more; and see not only the ‘wat’, but the ‘why’: is it a misunderstanding based on an assumption from another programming language? A compiler optimisation? A known bug that can’t be fixed due to backward compatibility concerns. Check her talk here. Guaranteed you enjoy and learn something!!</p>

## 11. The Packaging Lifecycle with Poetry by Clinton Roy

<p style='text-align: justify;'>
Clinton walks us through Poetry, Python dependency management tool with a very soothing pace. Based On the Poetry git hub page, the main reason to create  poetry is; </p>

{{< alert theme="warning" >}}
Packaging systems and dependency management in Python are rather convoluted and hard to understand for newcomers. Even for seasoned developers, it might be cumbersome at times to create all files needed in a Python project:setup.py, requirements.txt, setup.cfg, MANIFEST.in and the newly added Pipfile 
<cite>- Poetry Git Hub Page </cite>
{{< /alert >}}

<p style='text-align: left;'>
This is really true that there are many files we should consider such as:
</p>

- Setup.py
- Requirements.txt
- Setup.cfg
- MANIFEST.in
- Pipfile and Pipfile.lock (pipenv)

<p style='text-align: justify;'>
To solve this messy situation, Poetry comes here for us with only one pyproject.toml file to manage all the dependencies. This talk aims to look at some of the ways Poetry moves the conversation forward, learns from other packaging ecosystems, and where Python itself is going. Check here for Clinton’s talk!</p>

![free-food](/images/2019/free-food.png)

> Woop! Woop! Free food was served all the 3 days of the conference

## 12. Build and hack your own IoT with MQTT by Agnetha Korevaar

<p style='text-align: justify;'>
Today, we hear a lot about IoT, which stands for the internet of things. All these smart boxes, light bulbs, shades, thermostats, voice assistants, and smart machines are slowly sneaking into our households, businesses, and industrial environments. It’s a logical and inevitable next step, as we include more devices in our homes, that we develop some way to control them.</p>

<p style='text-align: justify;'>
When implementing the MQTT protocol, users set up a server. For consumers, the server usually lives on a PC or a mini-computer such as Raspberry Pi, to which devices can connect to and communicate with. While the MQTT protocol itself is secure, if implemented and configured incorrectly, severe security issues can arise. Agneta guides us to build our own IoT system and hack it to find out its weaknesses. Very informative!! Check here for her talk.</p>

