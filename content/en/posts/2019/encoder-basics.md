---
title: "Encoder Basics"
date: 2018-09-26T05:28:42+12:00
description:
url: /encoder-basics/
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
image:
---
<p style='text-align: justify;'>
I have come across encoders in my internship projects also personal projects such as Open barbell. Thought its better to draw something in a pencil regarding encoders which will help me to understand more about encoders while you can learn something too.</p>

<p style='text-align: justify;'>
The most common encoders are incremental encoders, for two main reasons. First, the information supplied by an incremental encoder is sufficient for most applications. The second reason is just a matter of economics and simplicity: it is much more cost-effective to manufacture an incremental encoder than an absolute encoder. An incremental encoder can be used in positioning and motor speed feedback applications which includes servo/light, industrial or heavy-duty applications.</p>

![encoder](/images/2019/encoder-1.png)

<p style='text-align: justify;'>
The above picture shows the very basic structure of an incremental encoder. It only involves a disk with one slot, an LED, and a photosensor. The detector provides an output each time it “sees” the LED.</p>

<p style='text-align: justify;'>
The first information an incremental encoder display is its output is distance. As the above disk rotates, each time the slot is aligned with the LED and detector, the detector produces an output. When the disk rotates through 360-degree mechanical degrees, the controller can use this information to calculate the distance traveled in a system.</p>

<p style='text-align: justify;'>
The second information an incremental encoder display is its output is velocity. the encoder essentially acts as a tachometer. As the disk in our first drawing above rotates, each time the slot is aligned with the LED and detector, the detector produces an output. The number of outputs in a minute would be the RPM or speed of the disk.</p>


<p style='text-align: justify;'>
How about with 10 slots and 10 teeth, the optical sensor can now provide an output while the disk turns through 18 mechanical degrees and a slot is in front of the sensor. During the next 18 degrees, a tooth will block the light, and the optical sensor will provide no output.</p>

<p style='text-align: justify;'>
Most applications need an output when the movement is much less than 18 degrees, so disks are made with much finer increments. The technical term used to define the size of increments used is resolution. I will discuss a resolution in more detail in a future post but for now, we can define it as the number of outputs provided by the encoder based on the number of lines or windows on the disk.</p>

![encoder](/images/2019/encoder-2.png)

<p style='text-align: justify;'>
Above drawing indicative of what that single output might look like on an oscilloscope. The bottom of the drawing represents an output of zero volts. The top of the drawing represents an output of five volts. The complete drawing is showing the changes in output or cycles as the disk rotates. When the sensor sees the LED, the output goes high (5 volts); when the disk via the line prevents the sensor from seeing the LED, the output goes low (0 volts).</p>

<p style='text-align: justify;'>
One complete electrical cycle starts when the output goes high and ends just before it goes high again. One electrical cycle is 360 electrical degrees. For every mechanical revolution, the number of electrical cycles will be equivalent to the resolution or lines and windows on the disk.
</p>

<p style='text-align: justify;'>
Although we are able to calculate both distances moved and velocity from a single encoder output, one other piece of information provided by incremental encoders is the direction of travel. In a future post, this will continue this discussion and explain how direction can be determined. This is just for a basic understanding of what and how incremental encoders work. Let me know if I made a mistake in the above post.. more than happy change or learn more…</p>

