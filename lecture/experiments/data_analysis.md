# Analyzing Experimental Data in Python

After spending quite a good while on important prerequisites concerning scientific computing and the basics of the `python` programming language, it's finally time to combine them via transitioning to more applied topics. This adventure will start with a brief exploration of how to create and run experiments using [PsychoPy](https://www.psychopy.org/index.html), a `python library` dedicated to conducting experiments in the realm of `psychology` and adjacent fields. Due to time constraints we will only have a quick look at things and showcase the most important aspects to allow folks to explore things further after the course ends. We'll further concentrate on using psychopy to further your understanding of the Python essential such as control-flow statements.

### Introduction to Experimental Work in Python Part 2 - Data Analysis, first steps

In this session, we will jointly go through a tutorial that shows us how to read in data using pandas, and do some simple corrections and first descriptive statistics.
     

### Materials 📓

You find the code for this session in the following [notebook](hhttps://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/lecture/experiments/intro_psychopy_2_data_analysis.ipynb)

You can download the data we need for this [here](https://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/lecture/experiments/pfp25_psychopy_data.zip). Please download them, put them into a convenient place on your computer, so that you can access them from jupyter by specifying the path to the data.


### Final Assignment: Modulpruefung

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




#### Submission of Assignment
Please e-mail the final notebook to fiebach[ at ]psych.uni-frankfurt.de.

**Deadline is March 15, 2026!**


## optional/reading/further materials

The official website of PsychoPy provides a lot of helpful information. For example, [here](https://www.youtube.com/@PsychoPy_official/videos) you can find video tutorials, on interesting topics like `Build your first PsychoPy experiment (Stroop task)`, `PsychoPy is Easy: Posner cueing task`, `How to copy and paste a routine in PsychoPy` or `How to check if a typed response is correct in PsychoPy`.  

There are many more resources ... Here, for example, you find the first video in an easy introduction series to PsychoPy:
<iframe width="560" height="315" src="https://www.youtube.com/embed/tTq6IfESVZs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

