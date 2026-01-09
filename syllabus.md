# Syllabus

In this course, we will overview the basics of optomechanics, lasers, and interferometers, 
with a focus on understanding optics lab components and gravitational wave detectors like Advanced LIGO.

## <span style="color: #7ba6f6ff;">Course Info</span>
- **Professor**: Craig Cahillane
- **Time**: Monday Wednesday, 12:45 - 2:05 pm
- **Location**: Physics 208

## <span style="color: #ff9c9c;">Course Topics</span>
1. Intro to Lasers
2. Plane Wave Mechanics and Interference
3. Interferometers
4. Gravitational Waves Detection
5. Geometric Optics
6. Transfer Functions
7. Fluctuation-Dissipation
8. Control Systems

and more Special Topics.

## <span style="color: #9cff9c;">Course Overview</span>

### Goals
A key component of this course will be familiarizing yourself with the latest interferometer simulation tools,
as well as understanding them analytically.
To do this effectively, we will need to rely on modern technical tools.
The hope of creating these interactive jupyter notebooks is to allow students in *Lasers and Optomechanics* to become familiar with tools used by scientists in the field of gravtiational wave detection.

### Textbooks
We will be relying on several texts and some video overviews
The major texts we will rely on are
1. *Lasers* by Seigman {cite}`Siegman_1986` [Free eBook](https://opg-optica-org.libezproxy2.syr.edu/content/bookshelf/book/item/lasers)
2. *Fundamentals Of Interferometric Gravitational Wave Detectors* by Saulson {cite}`Saulson_2017` [Syracuse Library Link](https://search.syr.edu/discovery/search?query=any,contains,fundamentals%20of%20interferometric%20gravitational%20wave%20detectors%20&tab=Everything&search_scope=MyInst_and_CI&sortby=date_d&vid=01SYU_INST:SYU&facet=frbrgroupid,include,9008347074956529785&lang=en&offset=0)
3. Some of the [*Feynman Lectures on Physics*](https://www.feynmanlectures.caltech.edu/)

Minor texts or articles will be clearly linked at the start of each lecture or homework as well.

### Evalulation
We'll have three major course components:
1. Homework
2. In-class Quizzes (every Wednesday)
3. End-of-year Special Topics Review Project by each student

The grade breakdown is as follows:
```{table} Grade breakdown for *Lasers and Optomechanics*
:name: table:grade_breakdown
:align: center

| **Component**  | **Percent of Final Grade** |
|----------------|------|
| Homework       | 30\% |
| Quizzes        | 30\% |
| Review Project | 40\% |
```
**Homeworks** will be due every two weeks on Friday.
I will release them on this course website in Jupyter Notebooks with questions that must be completed.

All homeworks must be turned in via Jupyter Notebook.
I recommend downloading the homework file from the gitlab: [https://github.com/ccahilla/lasers-and-optomechanics](https://github.com/ccahilla/lasers-and-optomechanics)

Most problems will require math to be done.
These may be done on paper and scanned in, 
or directly in $\LaTeX$.

Some problems will require plots be made. 
I recommend doing those in python in the notebook.

**Quizzes** will be a short in-class question reviewing the previous week's physics concept from lecture, readings, and homework.

The **End-of-year Review Project** will be to prepare a review in a Jupyter Notebook 
like the ones in this class about a topic in interferometry, lasers, optomechanics, or anything else related to the course.

### Videos
I have linked some useful optics videos in [](#table:videos).
These are not required for class, but in some cases strongly recommended to quickly review course content.

## <span style="color: #9c009c;">Prerequisites</span>

Students will be expected to have working knowledge of the following
1. Waves
2. Classical Mechanics
3. Complex Numbers
4. Differential Equations
5. Laplace Transforms
6. `python`
7. Linear Algebra

We will review topics as necessary, but previous exposure will be useful.

## <span style="color: #f0bf75ff;">Github Repo and Python Virtual Environment</span>

Below are instructions to create the `lasers` virtual python environment, which will allow you to run the jupyter notebooks which make up our interactive lectures.
I have included instructions for Mac and Linux terminal users. 
I will be adding material throughout the semester, so you may need to `git pull` the repo again over time.
Let me know if any of these instructions do not work for you.

If you use Windows, you may be able to try these instructions in VS Code or some other terminal simulator.  
Please come see me and we will work out something together for you and all Windows users (if you find a workflow that works for you, please let me know so I can record it here):

1. Install `git`: [https://git-scm.com/install/](https://git-scm.com/install/)
2. Install `mamba` (do a Fresh Install): [https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html)
3. You can test both install in terminal with `which git` and `which mamba`
4. Git clone the repo: `git clone https://github.com/ccahilla/lasers-and-optomechanics.git` (cloning vis CLI or SSH also acceptable.)
5. Move into the directory: `cd lasers-and-optomechanics`
6. Look for a file named `environment.yml`.  This should define the `lasers` conda/mamba python virtual environment that will run all the code in this class, including `numpy`, `matplotlib`, and `jupyter` libraries.
7. Create the `lasers` mamba environment: `mamba env create -f environment.yml`.
8. Activate the environment: `mamba activate lasers`.  
9. If successful, you should see a `(lasers)` preamble in your terminal.
10. Test your `lasers` environment.  Run `jupyter lab` in a terminal with `lasers` activated. 
11. Visit `http://localhost:8888` in your browser.  `jupyter lab` should launch a locally-hosted server which allows you to run jupyter notebooks or other python or markdown code in your browser.
12. Within jupyter lab, try opening `chapters/00_introduction.ipynb` and running the notebook (I like to use the "fast-forward" button to "Restart the kernel and run all cells").

## <span style="color: #75ddf0ff;">End-of-year review</span>

The **End-of-year Review Project** will be to prepare a review of a special topic in a Jupyter Notebook.
I would like the format to be similar to a guided journal club: 
a more in-depth dive into a difficult topic that we may have mentioned or glossed over.

I expect the review to be well-researched, including several references at the end of the notebook.
I also expect the notebooks to *run*.
They may run in our *lasers* mamba environment, or you may give alternate instructions for how to run your code.

I have grouped the topics below into different sections.
Feel free to suggest you are interested in to me as well.

### Rubric
I will be grading the end-of-year review on the following

1. Scientific motivation
    - Goals or importance of the topic
    - Applications or impacts 
2. Depth of technical detail
    - Critical Concepts
    - Equations
    - Illustrative Plots
3. References (number, quality, and use in the notebook)
4. Presentation 
    - 20 minutes in-class presentation


### Special Topics List
The following are options for the final end-of-year review.

**Facilities**
1. Laser Interferometer Space Antenna (LISA)
2. National Ignition Facility (NIF)
3. Filter Cavity at Advanced LIGO

**Scientific Equipment**
1. Xygo Interferometer
2. Hartmann-Wavefront Sensors
3. Fiber Lasers
4. Telescopes
5. Laser Cutters

**Scientific Concepts**
1. Pondermotive Squeezing
2. Holograms
3. Parametric Instability
4. Thermal Lensing in Optics
5. Optical Springs (Sidles-Sigg)

