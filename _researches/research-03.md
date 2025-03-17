---
title: "A Hybrid Approach for Guitar Technique-Based Transformation of Symbolic Notes into Solo-Style Tablature"
collection: researches
# category: conferences
permalink: /research/research-01
# excerpt: 'This paper is about fixing template issue #693.'
# date: 2024-02-17
# venue: 'GitHub Journal of Bugs'
# paperurl: 'http://academicpages.github.io/files/paper3.pdf'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---
<img src="/images/gt_transcription.png" alt="transcription" width="400"/>  
This is my current Master’s thesis research. Our goal is to generate expression-rich, solo-style tablature from symbolic note sequences. Unlike traditional guitar transcription research, which often assumes that the input contains a guitar sound, our work removes this constraint and focuses on transcribing non-guitar music into solo-style guitar tablature. This scenario introduces three important distinctions.  Firstly, because the source audio can be from any instrument, it often provides limited information beyond pitch. Secondly, there is not necessarily a single “correct” tablature, since the music was not originally played on guitar and therefore multiple valid fingerings may exist. This makes the problem more open and flexible, and thus more challenging. Thirdly, although solo-style music is typically monophonic, which might seem easier than polyphonic chord-based guitar arrangements, the decision-making process for a solo-style phrase must consider many additional factors, not just hand constraints. As a result, this can actually be even more difficult.
**The final thesis paper, evaluation results, and complete code will be published here after I finish my final thesis defense in late April 2025.**

<!-- ![tanscription](/images/gt_transcription.png) -->

Guitar tablature (tab) is a popular musical notation among many guitar players, as it provides additional useful information, such as fingering and playing techniques, beyond pitch. Guitar transcription systems offer guitarists an unlimited pool of practice materials when desired tablatures are not available or are difficult to find. The task can be divided into two subproblems: (1) extracting mono or polyphonic notes from audio and (2) arranging the extracted note sequence into a valid tab. Our work focuses on the second subproblem by proposing a hybrid method for the arrangement. Although some early studies use end-to-end Deep Neural Network
(DNN) models to directly convert audio to tab, our goal is to generalize this approach and expand its applicability, especially when the target music may not originally played on guitar or when only traditional scores are available instead of audio
files.
Many existing approaches focus solely on biomechanical constraints, which are indeed predominant in chord-based tabs, but they often overlook an important element in the solo-style tab: guitar-specific playing techniques (for example, bending, slide, hammer-on, and pull-off). These techniques serve not only as symbolic sound generators but also provide fingering guidance and convey the music’s emotional content. Therefore, we propose a hybrid system that consists of: (1) a DNN module that captures the latent connection between each note in a sequence and its possible corresponding guitar technique and (2) a heuristic module based on a optimal path-searching method conditioned on the technique predictions from the DNN.We expect our model to produce reasonable finger arrangements, annotate the
finger indices for each note, preserve the guitar’s unique expressive characteristics and implicit emotional nuances, and offer users a degree of customizability.
