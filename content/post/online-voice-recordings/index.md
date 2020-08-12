---
authors:
- admin
categories:
- Methods
commentable: true 
comments: true
date: "2020-08-12T00:00:00Z"
draft: false
featured: false
image:
  caption: 'Image credit: [**freeSVG.org**](https://freesvg.org/mic2)'
  focal_point: "top"
  placement: 1
  preview_only: false
lastmod: 
projects: 
share: true
subtitle: ""
summary: "Recently, I gave a talk on running multi-session studies online at the 2020 BeOnline conference. I mentioned that we had recently collected vocal responses online, but I didn’t have time to talk any more about it. Here’s a little bit more about my experiences."
tags:
- Data collection
- Research methods
- Word learning
title: 'Tools and tips for collecting spoken responses online'
---

Recently, I gave a [talk](https://www.emma-james.co.uk/talk/06-20-beonline/) on running multi-session studies online at the 2020 [BeOnline conference](https://beonline.research.sc/2020). I mentioned that we had recently collected vocal responses online, but that I didn’t have time to talk about it. So, here’s a little bit more about my experiences.

We collected spoken responses as part of a word learning study. 125 participants were recruited via Prolific, and listened to a spoken story containing made-up words. In each of three test sessions (same day, next day, one week later), we asked them to try and recall the made-up words. We presented them with the starting sound for each word, and asked them to try and speak the whole word that they had heard in the story. We were interested in which words participants could remember at each test point, scoring each trial as correct or incorrect.


## The tools

The experiment was programmed in Gorilla, and we collected spoken responses using the [“Audio Recording Zone”](https://gorilla.sc/support/reference/task-builder-zones#audiorecordingbeta). This zone is still in BETA testing (at the time of posting), which means that Gorilla are still ironing out a few issues. We did some thorough piloting and made it through relatively problem-free, but Gorilla have added some warnings of issues to be aware of.

The zone includes a “Test Mode” option, which is Gorilla’s built-in tool for participants to test whether their microphones are working. This mode creates a short recording of the participant’s voice and plays it back to them so that they can check they can be heard. Note that this relies on their honesty though -- there is no way for the software itself to check sound quality, or for you to know that recordings are OK before the participant proceeds. 

Within your experimental task, you incorporate the zone on the relevant trial screen as you would any other response zone in Gorilla, and set the option to “Record Mode”. This will record a short sound file for each trial, which can be ended by a button press or a timeout (you can see the various setting options in the [guidance](https://gorilla.sc/support/reference/task-builder-zones#audiorecordingbeta)). At the end of my experiment, I downloaded a short .mp3 file for each word trial for each participant. 

I use [CheckVocal](https://link.springer.com/article/10.3758/BF03192979) (Protopapas, 2007) for scoring each recording as correct or incorrect. CheckVocal is freely available software that was originally designed to process naming data from DMDX software. Although these recordings were collected via Gorilla, it still did the job for me (after converting the files to .wav first). You can download the software from [github](https://github.com/0avasns/CheckVocal). 

## The tips
OK, so I’ve only run one experiment -- I don’t have a HUGE wealth of knowledge to offer. But here are the steps I took (or would take next time!) to try and maintain data quality:  

* **Put a test mode at the very start of your experiment.** I put this even before the main study information and consent form, as no data is collected at this stage.  Ask participants to change their settings until their audio is clear. If they can’t get it to work, they can return to Prolific with very little time lost, thereby minimising expensive data loss for you.
*	**Repeat the test mode** before the recording part of your task. You might not need to do this, but I repeated the recording tasks in subsequent test sessions and wanted to provide an opportunity for re-adjustment if needed. Plus it doesn’t harm to be a little extra cautious!  
* **Create your own test recording.** The test modes don’t store any data for you, so I added my own test trial. I asked participants to speak “Take me to the task” before starting the experiment, which served three main purposes:  
    1) It gave me a quick reference trial to check before approving the participant's submission on Prolific. Checking data quality before approval provides an opportunity to query any issues  at a stage when participants are likely to respond.  
    2) It provided a reference trial for subsequent scoring. Blank sound files are very hard to interpret (see below), so evidence of the participant’s microphone working during that test session can be helpful.  
    3) It reinforced that sound recording was a vital part of the experiment, and that participants shouldn’t try to proceed without it.  
    + *(And an extra point – it was wonderful listening to all the kind strangers with their various accents asking to be taken to the experiment!)*  
* **Avoid blank sound files.** Empty recordings can be very hard to interpret: they tend to consist of only white noise, and/or might be very short. This leaves you with no idea whether the participant didn’t attempt a response or whether the recording didn't work properly. To help with this, we encouraged participants to attempt an answer if they could, and speak “don’t know” or “pass” if not. The majority of participants did this, but I think in future I would keep a reminder on-screen.  
* **Don’t expect a lab-based environment.** Before starting this experiment, I had an idealised view that I would be able to tell if a participant wasn’t in an appropriately quiet environment, and that it would be easy to exclude them on that basis. It isn’t. You have no real idea whether that faint music/television is in the same room and whether the participants can hear it through their headphones. You don’t know how distracted that participant is from the children screaming at each other (OK I might have had to exclude *that* trial…). You might even hear your participants take an extra moment to ask their co-habitant to be quiet. Then what?   
*	**…Think very carefully about the implications of background noise for your research question**, and remember that you will never have the same control as in the lab. This goes for any online study --- it just becomes more obvious when collecting sound recordings. Of course, you will ask that your participants are in a quiet environment where they are unlikely to be disturbed, but if this is crucial to your experiment then you will really need to spell out exactly what that means and think through your criteria for exclusion. For me, my main measure was the accuracy of the word remembered (response times didn't matter) and I had other ways to ensure that participants were engaging with the task. I was also comparing this experiment to one conducted with children in schools -- background noise and screaming children are pretty common occurrences there too.  

I think that’s all I can think of that might be helpful, but please feel free to leave comments with any further questions or your own tips and experiences. You can read more about the study in our [recent preprint](https://psyarxiv.com/vm5ad), or access the experimental tasks on [Gorilla Open Materials](https://gorilla.sc/openmaterials/104397).  

Happy data collection! 
