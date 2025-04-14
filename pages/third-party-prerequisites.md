---
title: Third Party Content Prerequisites
keywords: pre-requisites, prerequisites, requirements
last_updated: 9 November, 2017
sidebar: home_sidebar
permalink: third-party-prerequisites.html
folder: prerequisites
---


## Introduction

### Purpose of this article

This article presents a set of prerequisites and constraints to respect when adding a learning resource to the CKLS. Respecting these guidelines will ensure that the content launches correctly for your learners and that the tracking is recorded correctly by the platform. 

### Terminology

LMS | Learning Management System. Software to manage and distribute training courses with e-learning content. 
SCORM | Sharable Content Object Reference Model. This is a global standard that ensures that e-learning content created in various authoring tools can be imported and functions correctly in any learning platform. SCORM defines how the content should be packaged so that it can be imported in the LMS, and how the content can communicate with the learning platform. 
AICC | Aviation Industry CBT Committee. This is a global standard that ensures that e-learning content created in various authoring tools can be imported and functions correctly in any learning platform. It is the predecessor of SCORM but is still used actively by certain content providers.
SCO | Shareable Content Object. A SCO is the smallest content unit that can be launched and tracked by the LMS. 

## General prerequisites

### Workstation requirements

The CKLS application has certain requirements to ensure that the platform functions correctly for your learners. Ideally, the requirements for running your content should be aligned with the platform requirements to ensure that your content runs smoothly. 

### Security restrictions

Executable files and files that contain server-side code can not be uploaded to the platform for security reasons. 

Some examples: .htaccess files, .php, .phps, .phtml, .pl, .cgi, .exe, .sh

If your content package contains one of these files, you will not be able to upload it as a learning resource. 

### Network constraints

You can upload content packages and files up to 200 MB via the CKLS back office. If your content files are exceeding that limit, we can provide you with a sftp account to allow you to upload larger files. Please get in touch with your Client Success team if you would need this. 

We recommend aligning the size, quality, resolution… of your content files to the network configuration of your target audience. For example, if you have mainly learners that will access your content via a slower mobile connection, you might want to adjust the quality of your graphics so that they still load smoothly on a slower connection. 

## Supported learning standards

### General compatibility

CrossKnowledge Learning Suite is conformant with the following standards: 
- AICC
- SCORM 

### Content metadata

The CKLS allows you to specify additional metadata for your learning resources. It is highly recommended to provide this metadata as it increases the findability of your content in the platform: 
- Title
- Author
- Description
- Theoretical duration
- Level of difficulty (1/2/3)
- Learning goals for the content
- Thumbnail picture (640 x 360 px)

### Tracking data

The following information will be available in the CKLS reporting for the standardized content: 
- Time spent
- Status (not started / incomplete / completed)
- Score

## SCORM specifics

### Supported versions

CKLS supports SCORM 1.2 and SCORM 2004. 

For SCORM 2004, we support the different “editions”, but as many LMSes we did not implement all of the optional runtime commands, especially the specific navigation and sequencing commands (for example adl.nav.request).

### Recommended format

We recommend using SCORM 1.2 “single-SCO” packages as the delivery format. 

Please ensure that the manifest file (imsmanifest.xml) is in the root of your zip archive, so that it can be read by the CKLS import routine. 

### Multi-SCO content

Although not recommended, the CKLS will accept multi-sco content. A navigation menu will appear on the left of the content so that the learner can navigate between the different SCOs. 

### Bookmarking

The CKLS will store the suspend_data so that a learner that leaves the content will return to the page where he left off on the next visit. 

Please note that SCORM 1.2 specifies a maximum of 4096 characters for suspend_data. If your content would send more than 4096 characters, we suggest publishing your content as SCORM 2004 3rd or 4th edition, which allows 64000 characters. 

### Progression

SCORM 1.2 uses the lesson_status to track the progression of the learner. The visual progress bar in the CKLS will indicate 3 possible states for your learning resource: 
- 0% => Not attempted
- 50% => Incomplete
- 100% => Completed

In SCORM 2004, you can use cmi.progress_measure to have a more granular progression.  

## Good practices

### Content duration

The CKLS allows you to create “collections” of learning content, either in a “self service” format (Learning Channels) or in a “guided” learning path (Blendedx course). Therefore, we recommend that the duration of your learning resource should not exceed 30 minutes. If your content is longer than that, we recommend splitting up your content in different small chunks. This will improve the experience for your learner and will also give you a more granular view on how the learner progresses in your content. 

### Committing your SCORM tracking

When your content communicates with the CKLS via SCORM, the tracking data is only saved (“committed”) when the content calls the function LMSCommit. 

We recommend committing the SCORM data on a regular basis, for example when a learner moves to the next chapter in your content. In case of an occasional connection loss, this ensures that recent data is kept, and the learner does not loose too much data. 

However, to protect our infrastructure from content that would be flooding the SCORM interface with excessive LMSCommit commands, the CKLS has a “5 second buffer” for commits: if a content sends two or more LMSCommit commands within a period of 5 seconds, only the first commit will be accepted. The other data will be buffered. Only changes in the lesson_status will be accepted on every commit. 

### Testing SCORM content

The CKLS has a specific SCORM Test Environment that allows you to test your SCORM content. You can upload the content, view the SCORM logs and verify that all tracking data is sent correctly. This will ensure that your content is communicating correctly with the CKLS before you open the course to your learners. 

Please contact your Client Success team if you would need assistance doing this. 

## Mass upload of content

The CKLS allows the upload of content packages “in bulk” in case you would like to import a large third-party catalog. 

Please contact your Client Success team if you would need assistance doing this. 
