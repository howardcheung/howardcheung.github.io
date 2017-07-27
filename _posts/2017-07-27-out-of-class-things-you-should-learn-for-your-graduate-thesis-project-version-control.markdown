---
layout: post
title:  "Out-of-class Things that You Should Learn for Your Graduate Thesis Project: Version Control"
date:   2017-07-27 23:10:00 +0800
categories: ["Graduate Study Tips"]
comments: true
---

Throughout my graduate study, there are lots of things that I have learned, and there are lots of things which I would like to learn much earlier than I did. One of these things is a proper version control scheme.

# So what is version control?

Version control, by [Wikipedia](https://en.wikipedia.org/wiki/Version_control), is the management of the change to documents, computer programs, large web sites, and other collections of information. A proper version control can help you to manage lots of versions of documents by keeping track of the changes of the files and the objectives of the changes and allow you to develop your projects in a more efficient manner.

# Q: Why do we need to do it properly? If I need a new version, I just save it as another file and call it version 10.

If you keep saving your files as new versions, at the end of your graduate study, with all the changes to your projects requested by your supervisors, committee members, project sponsors and paper reviewers, you will end up with a lot of files.

![](../../../../raw_img/GraduateStudy/NumFiles.png)

_Number of files of different versions for a thesis research. More than 200 versions and more than 6,000 files._

With version control, you can limit your number of files in your directory to ones of the current version:

![](../../../../raw_img/GraduateStudy/NumFilesWithVersionControl.png)

_Number of files of different versions for a project with version control. 248 files in total with a version control log for 216 revisions._

and revert back to other milestones whether necessary:

![](../../../../raw_img/GraduateStudy/ChangeBranch.png)

_Switch to an older branch when the current development direction is bad with just a few clicks_

For the project without version control, there're so many files without proper logs and revision numbers that you'll forget what they are. If you find your development direction to be useless and would like to go back to a previous file to start from scratch, do you know which file you should start from?

# Q: I have good memories. I can remember all of my work.

You can definitely remember its details when you're working on the project. But will you be able to remember what they are after you finish it for 2 months? How about 6 months? 8 months? Academia is a place where your work is tagged to you. Instead of a junior colleague who will follow up for you in the future, you will take care of your thesis project for the rest of your life if somebody asks questions about it. After 2 to 5 years, if somebody asks to replicate your work, will you be able to find the appropriate files to let them do so? If you keep staring at your files, you will eventually recall what you have done and give them the right files, but it will probably take hours to do so. With proper version control, a few minutes will be sufficient to give you enough log to recall what you have done for different versions.

![](../../../../raw_img/GraduateStudy/LogDiagram.png)

_A version control software showing a summary of past development directions and which version of files are residing in your directory now._

# Q: I am leaving the academia after graduation. I am not going to reply to anybody's questions about my work.

True. But some new graduate students in your graduate supervisors' research group is going to pick up your work, right? They are going to work on your materials for another 2 to 5 years. Will you be able to refuse to answer their questions related to your work in these years?

# OK. So where can I learn it?

If you do not want to use any new software tool, you can probably do it yourself by writing very good logs with all of your files and changes to the files. There are people who manage to do it this way (e.g. software source code with good comments). I am unfortunately not one of them, and I cannot give you tips on how you can learn the skills.

If you would like to use a software tool, you can start with ones with a graphical user interface (GUI) like [SourceTree](https://www.sourcetreeapp.com/), [TortoiseGit](https://tortoisegit.org/) or [TortoiseHg](https://tortoisehg.bitbucket.io/). If you're familiar with programming and would like to use the terminals/ command windows for more flexible and less computational expensive tools, you can use the tools behind these GUI such as [Git](https://git-scm.com/) or [Mecurial](https://www.mercurial-scm.org/). These free tools work best with plain text files and work fine with other types of files as well. There are also tools that are specifically designed for other types of files, but I have not used them and I cannot comment on their performance.

![](../../../../raw_img/GraduateStudy/GitExample.png)

_Using Git to record what changes have been made_

# Summary

With version control methods to manage your files for your projects, you can

* Limit the number of files in your directory. Only show the files of the current version.
* Revert bad work in progress and start your new development direction easily.
* Keep track of your changes.
* Set up a log to remind you what you have done in the future.
* Help answering questions related to your work after your graduation.

# TL;DR

Version control helps to manage the files in your directory by limiting the number of files in your site, helping you to revert your bad work quickly, keeping track of your changes to your project, and reminding you what you have done. So it's good to bookkeeping big individual projects like your graduate thesis project.
