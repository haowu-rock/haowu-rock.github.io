---
title: "Real-time Distortion Stacking Application"
excerpt: "(March 2024 - April 2024) This is my final project for the course 15622 - Introduction to Computer Music at Carnegie Mellon University in Spring 2024. It is a real-time distortion stacking application/plugin that enables users to combine various clipping functions to create custom distortion sounds. <br/><i>Click the title to see more details.<i/> <img src='/images/dist_block.png'>"
collection: portfolio
---

This is the Github link for the code: <a href="https://github.com/haowu-rock/DiskBlock" target="_blank">Github</a>  

The intention of this project is to create a real-time distortion experimental platform that enables users to design their own unique distortion effects using basic distortion building blocks (currently, it only provides several clipping functions). The application also includes features such as a real-time changeable signal chain, real-time adjustable parameters, input/output RMS meters, and a Fast Convolution block for loading Cabinet IR or Reverb IR.  

There are two videos recorded in April 2024 that compare the unprocessed dry sound of the guitar with the processed sound that has passed through this plugin.
For the processing settings, I randomly stacked several different clipping function blocks and then passed the signal through two fast convolution blocks using one Guitar Cabinet IR and one Hall Reverb IR, respectively.  

<!-- **Unprocessed:** -->
<h3 style="margin: 0;">Unprocessed:</h3>
<video width="560" height="400" controls>
  <source src="/files/unprocessed.mp4" type="video/mp4">
</video>

<h3 style="margin: 0;">Processed:</h3>
<video width="560" height="400" controls>
  <source src="/files/processed.mp4" type="video/mp4"> 
</video>  

<br/>
<h2 style="margin: 0;">This is the project manual created in April 2024:</h2>
<iframe src="/files/DistBlock_Manual.pdf" width="100%" height="800px"></iframe>
