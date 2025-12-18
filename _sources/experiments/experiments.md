# Running experiments in Python

After spending quite a good while on important prerequisites concerning scientific computing and the basics of the `python` programming language, it's finally time to combine them via transitioning to more applied topics. This adventure will start with a brief exploration of how to create and run experiments using [PsychoPy](https://www.psychopy.org/index.html), a `python library` dedicated to conducting experiments in the realm of `psychology` and adjacent fields. Due to time constraints we will only have a quick look at things and showcase the most important aspects to allow folks to explore things further after the course ends. We'll further concentrate on using psychopy to further your understanding of the Python essential such as control-flow statements.

### Introduction to PsychoPy - I

Most of us already conducted or at least watched or helped conduct an experiment. However, there's a fair number of different software options and tools out there, which mostly depends on the computational infrastructure at hand, but also on what people have the experience and skills to master - or simply what they used to use in the past. Often, these other solutions are not `open source` but paid software.

That being said: We'll quickly discuss some tools to conduct experiments and work out if we can actually use `python` based resources in this context with a clear conscience or if you're better off by defaulting to paid software packages.

To get some idea on how to present experiments via Python, we will explore the `python library` [PsychoPy](https://www.psychopy.org/index.html), including its setup, basic working principles, as well as advantages and disadvantages, showcased on a very simple experiment. Buckle up y'all, this is the first time we will use `python` "in the wild".      

### Materials 📓

In case you have not yet done so - please install `PsychoPy` from [here](https://www.psychopy.org/download.html).

You can download the slides for todays session [here](https://docs.google.com/presentation/d/1Sjo6YW92Ju_Zk5_glrQZpFsBNYYD88fTy2vYziZ1wR4/edit?usp=sharing)

In this session, we will jointly go through a tutorial, implementing a simple rating task - led by Dr. Cosimo Iaia from our research group. As homework assignment, you will adjust this experiment to work with different stimuli.  

You find the code for this session in the following [notebook](https://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/lecture/experiments/intro_psychopy_I.ipynb)
**However -  you should not try to run the code in the jupyter notebook! We will copy and paste it into the `PsychoPy coder`.**
You can also access the pre-rendered version of this notebook through the table of contents on the right.


**Remember: For this, you need to have installed PsychoPy as a stand-alone program! The `PsychoPy` code does not and should not be run in jupyter notebooks - we will use `coder`, i.e., a code editor that is provided with `PsychoPy`.**


### Homework assignment #7

Your next homework assignment will entail the generation of a “new” psychopy experiment. You can use the tutorial as a starting point. Your new experiment should include a trial sequence where some stimulus is presented and a response is collected. 

Please implemente a rating task using the words below, asking participants to rate **on a scale from 1 to 9** how concrete (1 = very concrete) vs. abstract (9 = very abstract) these words are. 

Words: Felsen, Gabel, Apfel, Hammer, Frieden, Ruhm, Pfanne, Ehre, Anker, Stuhl, Wahrheit, Tragik, Seele, Hoffnung, Besen, Toaster, Weisheit, Klugheit, Bagger, Liebe. 

These words come from this paper: Kanske, P., & Kotz, S. A. (2010). Leipzig affective norms for German: A reliability study. Behavior research methods, 42(4), 987-991.

Please use a dialogue box to ask for participants`s age, handedness and initials (as a subject ID). 

Please also adjust the instruction in the start message to the new task.

Please add a fixation cross for 1000 ms after the response was given.

The output file should automatically be named after the participant ID. 

The script should write the results of the rating task, including the chosen value and the response time as well as the item itself, the item number and the handedness of the participant into an output logfile (csv). Please think about the most reasonable order for the variables for this output, and implement it.

You can (and should!) implement all of this inside the Psychopy Coder!

Note that: 
- Your script should run without crashing and generate an output file. 
- Remember: It should have a dialogue box where partcipants can input e.g., id (initials of your first and last name), age, handedness which will be written to the output file

Save the experiment script as a .py file that contains your name in its filename.

#### Part 2:
Please run the experiment and send the output file also. We want to assemble all output files into dataset after the winter holiday and analyze the acquired data.

#### Submission of Assignment
Please e-mail both files to fiebach[ at ]psych.uni-frankfurt.de.

**Deadline is Monday, January 12, 2026!**


## optional/reading/further materials

The official website of PsychoPy provides a lot of helpful information. For example, [here](https://www.youtube.com/@PsychoPy_official/videos) you can find video tutorials, on interesting topics like `Build your first PsychoPy experiment (Stroop task)`, `PsychoPy is Easy: Posner cueing task`, `How to copy and paste a routine in PsychoPy` or `How to check if a typed response is correct in PsychoPy`.  

There are many more resources ... Here, for example, you find the first video in an easy introduction series to PsychoPy:
<iframe width="560" height="315" src="https://www.youtube.com/embed/tTq6IfESVZs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

