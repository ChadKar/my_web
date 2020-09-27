---
title: "I Screw Up My First Open Barbell"
date: 2018-11-25T02:09:05+12:00
description:
url: /open-barbell/
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: inner
tocLevels: ["h2", "h3", "h4"]
tags:
- Gadgets
- Technology

series:
- 
categories:
- Gadgets
- Technology
image: /images/2019/OB_pcb2.png
---

<p style='text-align: justify;'>
Companies are making efforts to calculate barbell path and system performance with the body and barbell, and even measure for the rate of force. Barbell speed trackers allow us to account for this: they provide an instant, measurable metric that can be used to determine how much should actually be lifted. If we feel fatigued and sluggish but are actually moving the barbell at a good speed, this information becomes invaluable. Instead of dropping weight or calling it early, we can go up in weight. Compounding from session to session, this small percentage gain <a href="[url](https://pubmed.ncbi.nlm.nih.gov/21311352/)">can make a huge difference</a> in the course of a training cycle. 
</p>


<p style='text-align: justify;'>
Coming from an Embedded background I always wanted to make my own Velocity Based Training(VBT) device to track my training progress.Obviously, it needed to be a low-cost, accurate, and reliable platform to measure important information about barbell exercises. OpenBarbell from Squat and science is one of the accurate devices in the market. Their OpenBarbell version 1 unit is open-source.
</p>

## My Approach to Open Source Embedded Project

<p style='text-align: justify;'>
So I decided to dig this project and make my own barbell VBT unit. Even though the original project is 5,6 years old. Open barbell GitHub account is still live with the all the PCB,3D mechanical drawings.</p>

<p style='text-align: justify;'>
After research the project I found that most of the components were obsolete. So I straight downloaded the project from GitHub and see if I could hack the code. I found all the libraries and whatnot (this part will discuss in the future how I go with Arduino C and their mobile app.) The next mission is to find the obsolete component. After sniffing few electronic forums I managed to found that if I dig deep from electronic manufacturers in Hong Kong, China and the US we may have a chance. After 2 months and about 20 emails, I found a lead that a couple of manufacturers in China have the main microcontroller(RFDauino) which is the ‘brain’ of the Open barbell.
</p>

## What Went Wrong
<p style='text-align: justify;'>
Things started to fall from here.I was too lazy maybe too dumb.Haven’t check Open-barbell old PCB file. Straight contacted the one manufacture in China and asked them to manufacture the board, sending the fresh Gerber file I made from the OpenBarbell Git-hub account.Paid for 3 board to populate. It took four weeks to manufacture the board. After a hefty customs charge from NZ custom, boards were finally on my hand.</p>

![ob_pcb_1](/images/2019/OB_pcb1.png)

<p style='text-align: justify;'>
I was over the moon! It was time to test the board! I fired up the board. None of them were alive means that fun time starts. Its fault-finding time. Alright peeps this is what I learn from this part of the project.Their Schematics missing the two capacitors also BOM I download from git have resistor and capacitor values are mismatch from the schematic diagram! Am I screwed! Not really but should have done better if I follow the below steps. Here I am making my own standard for my next Open source Embedded project:
</p>

## What  Can We Learn From My Mistakes

1. Check the availability of software libraries and understand the code. (which I have done for this one)
2. If the project has a mechanical side how feasible how easily we can build it. (Already done this one)
3. Always check the schematic make sure you understand the whole circuit. Download all the data sheets and see the schematics are correct! (This where I missed)
4. Check the Gerber file before you send it to manufacture.
5. Alaways Try to populate the board myself if SMD Components aren’t too small! (I was lazy for this project. Should have save that hefty custom Fee, component populate charge if I solder the board in the house)


![ob_pcb_2](/images/2019/OB_pcb3.png)

<p style='text-align: justify;'>
What am I gonna do now? Well, debug the board sigh!!Stay tuned how I debug the board…You’ll learn something…also basic mechanism of this open barbell project is that the conveying draw-string mechanism through an encoder wheel. Check encoder basics if you want to learn more about encoders.</p>


**Part 2: To be continued....**

