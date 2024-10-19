---
title: "Cross-platform Audio Framework FUSION"
excerpt: "(June 2021 - November 2021) FUSION is a cross-platform C++ application framework that enables developers to create audio-based applications for desktop (Windows/Mac) and mobile (iOS/Android) platforms without needing to worry about the underlying audio routing. <br/><i>Click the title to see more details.<i/>" #<img src='/images/500x300.png'>"
collection: portfolio
---

I led this project and designed the structure and interfaces of the framework. I implemented the virtual classes and functions for iOS and macOS systems, while other colleagues implemented theirs for Android and Windows. Developers can easily plug in or swap their algorithm modules to process audio signals. Essentially, it functions like a lightweight version of JUCE, excluding many unrelated features, such as the UI components, and is customized specifically for Rantion Technology for internal use.  
 
*Since the code is proprietary to the company, I can only share a general structure and an example of its usage.*  

**General Structure**
![fusion_frame](/images/fusion_frame.png)

**Code Snippet for Using FUSION Framework**  
Different RenderUnit classes represent various real-time audio processing algorithm modules.
![fusion_use](/images/fusion_use.png)