---
project: Belle2
title: Advanced Belle II Software Validation
author: Arul Prakash
[//]: # (photo: blog_authors/FirstLast.jpg)
date: 28.07.2022
year: 2022
layout: blog_post
logo: belle2-logo.png
intro: |
  The Belle II Software suite is the custom software tasked with handling the simulation, reconstruction and analysis of the data coming in from the Belle detectors. Belle II Software has had several monitoring schemes implemented so far, along with a high-level validation tool. This project seeks to enhance the user experience of the Belle II software validation page and make workflows more efficient with appropriate technical solutions.
---

The Belle II Software suite is the custom software tasked with handling the simulation, reconstruction and analysis of the data coming in from the Belle II detector. To keep pace with the current research and technological evolutions, the code undergoes constant changes, to optimize the algorithms for better physics performance and to ensure resource efficiency.

The Belle II software has had several monitoring schemes implemented so far, along with a high-level validation tool. This tool runs on existing large datasets producing distribution plots of quantities relevant for physics analyses and displaying the results on a webpage. This project seeks to enhance the user experience of the Belle II software validation page and make workflows more efficient with appropriate technical solutions.

### Problem Outline

These are the things that can be improved upon, in the existing system.

 * Proper tracking of degradation history with the help of bookkeeping software.
 * Having references inside plots generated by the validation system.
 * Make it easier to find associated artefacts to encourage reuse.
 * Provide developers with more information about failures found to help with root cause analysis. 


### Journey so far

 #### Local base
 Initial days were spent setting up the basf2 software in the local system to be able to run the validation tool, host a local validation server and as well as to develop the code. Relevant data files were also obtained that are necessary inputs for certain validation modules. Finally, a Gitlab project was set up to mimic the production project and to be a playing field to test initial implementations. 

 #### Code review 
 Whilst the base was being built on the sideline the existing implementation review was underway. The first aim was to get a birdseye view of the overall system and then do a deep dive into the relevant modules, and identify the modules of interest. Time was also spent familiarizing myself with the software development and coding conventions. 

 #### CherrPy meets Gitlab
 Two of the key tech that will feature throughout the work are CherryPy and Gitlab, so a good amount of time was spent understanding and then getting hands dirty with trying and testing the integration of the two, which is key for the bulk of the improvements planned. With that, the first task undertaken was to extend details displayed along with plots of validation runs to include a list of relevant issues. A couple of features have also been added that would allow the reviewer of the results to directly create issues from the plot display window or update existing relevant issues in Gitlab. 

### Perosnal experience
So far it has been a learning ordeal that I have thoroughly enjoyed, and am looking forward to stepping up and making more meaningful contributions. I am extremely grateful for all the support I have been receiving from my mentors. I was provided with the platform to explore new ideas. An added bonus was being able to take part in the regular software development meeting to get to know about the other work being done as well and present and receive feedback on my  implementation as well. Overall an enriching experience so far, and having had a foretaste I'm sure of the same if not more in the second half of the stint. 

#### Links
 * [Project proposal](https://hepsoftwarefoundation.org/gsoc/2022/proposal_Belle2Validation.html)
