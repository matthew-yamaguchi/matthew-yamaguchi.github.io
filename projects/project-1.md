---
layout: project
type: project
image: images/ics_111_actor.png
title: ICS 111 - Animation Program
permalink: projects/ics111_actor
# All dates must be YYYY-MM-DD format!
date: 2016-10-30
labels:
  - Java
  - Animation
  - C++
summary: An animation project created during my ICS 111 class at UHM.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/ics_111_actor.png">
</div>

During the fall of 2016, I took ICS 111 at UHM.  We were assigned a project to create a class that involved animation.  The class required an image parameter and had functions that allowed it to move to a specific coordinate on the screen and rotate to a specific angle.  We further modified the class to be able to read from a .txt file.  Based on commands and coordinates in the text file, the "actor" object would carry out what we wished it to do.

This was an individual project and all code in this program was created by me, excluding the EZJava.txt file.  

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



