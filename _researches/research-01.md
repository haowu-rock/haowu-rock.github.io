---
title: "Guitar Chord Recognition Algorithm"
collection: researches
# category: conferences
permalink: /research/research-03
# excerpt: 'This paper is about fixing template issue #693.'
# date: 2023-05-1
# venue: 'GitHub Journal of Bugs'
# paperurl: 'http://academicpages.github.io/files/paper3.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---
<img src="/images/guitar-chord-recog.png" alt="transcription" width="400"/>  

This project was a preliminary research initiative aimed at exploring potential future products for Guangzhou Rantion Technology Ltd., where I worked as an Audio Algorithm Engineer from 2021 to 2023. I designed a real-time guitar chord recognition algorithm using DSP techniques and contributed to research on non-real-time music chord recognition, leveraging machine learning methods. Rantion Technology Ltd. has patented this algorithm. Click the title for more details.

## 1. Real-Time Guitar Chord Recognition Algorithm 
This signal flow diagram illustrates the general processing steps involved.

![DSP signal flow](/images/Chord_Recognition_DSP.png)

**Downsampling:** Downsample the input to a lower sampling rate and filter out frequencies that cannot be produced by a guitar.  
**Onset Detection:** Detect the onset of each chord event and utilize a short audio segment following a successful onset detection to predict the corresponding chord.  
**Feature Extraction:** Compute the chromagram for the audio clip.  
**Feature De-noising:** The primary goal is to reduce interference from the harmonic frequencies of each note.  
**Pattern Matching:** Match the features with a pre-defined chord matrix to calculate scores for each candidate and select the one with the highest score.  
**Correction:** This step addresses the issue of mismatched chords, as the same notes may belong to two different chord classes, such as normal triads and 7th chords or diminished chords.

**Recognizable guitar chord types:** major triads, minor triads, augmented triads, diminished triads, suspended 2nd chords, suspended 4th chords, major 7th chords, minor 7th chords, dominant 7th chords, and minor-major 7th chords.


The project is proprietary to the company, so I am unable to share the code. However, there is a demo video recorded in 2022 showcasing the application built on this algorithm. In the video, I am demonstrating the algorithm's functionality by playing the guitar.
<video width="640" height="360" controls>
  <source src="/files/ChordRecognition_DSP.mp4" type="video/mp4">
</video>
*This video demonstrates chord recognition using DSP techniques. I am the person in the video!*

## 2. Non-Real-Time Music Chord Recognition Using Machine Learning
This is a chord recognition method based on the LightGBM 

**Recognizable guitar chord types:** major triads and minor triads (first version model was trained using only these two labels).

Another demo video, recorded in 2022, showcases the capabilities of the machine learning algorithm. In this demo, we load a song along with its corresponding label file. Once the analysis is complete, the predicted chord labels are displayed alongside the correct labels, both aligned with the audio waveform at the bottom of the screen.
<video width="640" height="360" controls>
  <source src="/files/ChordRecognition_ML.mp4" type="video/mp4">
</video>
*This video demonstrates chord recognition using Machine Learning techniques.*

