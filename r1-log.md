# #100DaysOfCode Log - Round 1 - Johannes Stutz

The log of my #100DaysOfCode challenge. Started on **January 30, Saturday, 2021**.

## Log

### R1D1 
Started a [Python website blocker](https://github.com/JohannesStutz/python-website-blocker) / productivity script. Have a prototype running. Ideas for many features, i.e., scheduling and Pomodoro. Not sure if Python is the right tool, a standalone tool or browser extension would be better.

### R1D2
Didn't have much time for coding today. Continued with [Python website blocker](https://github.com/JohannesStutz/python-website-blocker) and added a Pomodoro timer. Next: feature for scheduling or blocking websites for a specific length of time. Also: figure out how to make an installable package.

### R1D3
- Decided to try the website blocker project with [nbdev](https://github.com/fastai/nbdev). A tool that lets you develop software in Jupyter notebooks. It can automatically create pip packages and a documentation website: https://johannesstutz.github.io/beproductive/
- GitHub link: [Be Productive](https://github.com/JohannesStutz/beproductive)
- Added support for Linux (and probably MacOS, can't test it)
- Had trouble using git. Took over half an hour to fix a merge conflict caused by A SINGLE LINE. Need to learn git basics!

### R1D4
Had not so much time today. Tried to turn [Be Productive](https://github.com/JohannesStutz/beproductive) into a proper command line tool. Learned about `argparse`. You can now run `python -m beproductive pomodoro` and a Pomodoro session starts. Next up: scheduling / block websites for certain time. Git was better today :)

### R1D5
Skipped because of my birthday :)

### R1D6
Added the option to block websites for a certain time. `python -m beproductive block 45` blocks all websites for 45 minutes. Also, you can customize Pomodoro times. `python -m beproductive pomodoro 30 10 4` runs 4 Pomodoros of 30 minutes with 10 minute breaks.
Tried to create a pip package, but could not get nbdev to work in WSL2

### R1D7
Made a [PyPi package](zyDMg7LPSaa7)! `pip install beproductive` is enough to get the package running. 

### R1D8
New project: Blurry. A privacy tool that automatically blurs faces in photos (and maybe videos). Developing in nbdev again. [First notebook](https://github.com/JohannesStutz/blurry/blob/master/00_core.ipynb) is very rough but proof of concept.

### R1D9
Played a bit with webcam and Blurry. Prototype for live face blurring. Works okay, although with very low framerate (~10fps). Next week: build a command line tool for image processing. Maybe web app.

### R1D10
New project: blur the background in webcam videos. [Link to repo](https://github.com/JohannesStutz/background-detection). Very productive day! Starting with taking images, annotating them, building a model with fastai and writing some OpenCV code to create a video with blurred video. Blog posts not quite finished yet but coming along.

### R1D11
Spent a lot of time finishing the [blog post](https://deeplearning.berlin/fastai/privacy/getting%20started/2021/02/09/Background-Blur-Part-1.html) for background blurring. Part 1 is online. Figured out a better way to do the masking (alpha blending instead of binary mask), will cover this in blog post no. 2 tomorrow.

### R1D12
Released [blog post part 2](https://deeplearning.berlin/fastai/privacy/opencv/2021/02/10/Background-Blur-Part-2.html) for the  background blurring project. Not too much actual coding today, but improved inference process. No more writing frames to disk but passing them directly to the model! Tomorrow it's back to the Website Blocker.

### R1D13
Worked on the Be Productive project, the website blocker. I want to implement customization of the URLs via command line. So far not too much progress, learned about config files but I'm struggling with implementation. I don't get importing between modules... Will try refreshed tomorrow
