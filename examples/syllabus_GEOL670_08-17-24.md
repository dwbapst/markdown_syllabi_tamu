# Syllabus

<!--
This is a syllabus template in Markdown that meets the minimum syllabus requirements made by the Texas A&M Faculty Senate beginning in Fall 2020. The Markdown format (a .md file, as denoted by the file name) used in this document was chosen to maximize conversion to HTML or PDF via Pandoc. This Markdown-based syllabus template is based on the original template written for use in Microsoft Word. The conversion to Markdown was done by David Bapst in the College of Geosciences.

The accessibility requirements for syllabi includes a single level-1 heading (i.e., “Syllabus”) with three level-2 headings (i.e., “Course Information,” “University Policies,” and “College and Department Policies”). The “Course Information” and “University Policies” sections have subsections identified with level-3 headers (and occassionaly their own subsections with level-4 headers). 

To use this syllabus template, faculty should edit the content in the “Course Information” sections to include the appropriate details for the course, and review the text included in the “University Policies” section. The TAMU Faculty Senate established the wording of the text in this section. Faculty associated with the main campus in College Station should use the Academic Integrity, Americans with Disabilities Act, and Title IX statements as written. Faculty not on the main campus should use the appropriate language and location at their site for the Academic Integrity, Americans with Disabilities Act, and Title IX statements. NOTE: Faculty members should not change the written statements. A faculty member may add separate paragraphs if additional information is needed. Faculty should also add subsections for college level and/or department level policies as appropriate for their respective units. Faculty should use Heading level-3 (in Markdown, denoted by a line beginning with three hash symbols: ###) for any new headings added under the College and Department Policies section. 

The template can then be converted to HTML using Pandoc, which can be obtained here: https://pandoc.org/

To use this syllabus template for creating a PDF, you must also have a LaTeX engine installed and in your system's $PATH. If you are on a Linux machine, you probably have such, or can easily obtain such from a software package repository. This is somewhat more difficult on macOS or Windows, although if you have RStudio installed and often convert Rmarkdown files to PDF, you *may* already have the requisite software installed. To convert this file to a standard LaTeX-style PDF, all you need to do in the shell is (assuming your working directory contains the file in question):

EXAMPLE

pandoc syllabus_template_07-19-21.md -o test_syllabus.pdf --variable urlcolor=blue

RUN THIS:

cd ~/teaching/GEOL670_GeolDataAnalysis_Fall2022/syllabus/
pandoc syllabus_GEOL670_08-25-22b.md -o syllabus_GEOL670_08-25-22b.pdf --variable urlcolor=blue
okular syllabus_GEOL670_08-25-22b.pdf 2> /dev/null &

Converting to HTML

pandoc syllabus_GEOL670_08-25-22b.md -o syllabus_GEOL670_08-25-22b.html

What is this stuff I'm reading?

The text you are reading is plain-text comments within HTML commenting -- this text does not appear when the Markdown file is converted to HTML or PDF. HTML commenting blocks are designated with a  <!-- at the start, followed by two dashes and an end symbol Multiple such commenting blocks are allowed. Because commented text is ignored, you can delete these lines, leave them be, or even add additional comments throughout the document for your benefit.


The following is a YAML header designated by --- above and below.
The command in the YAML header following makes sure that margins are 1 inch in latex PDFs
-->

---
geometry: margin=0.5in
---


## Course Information

Course Number: GEOL 670

Course Title:  Geological Data Analysis 

Time:          2:20 - 3:35 PM, Tuesday/Thursday

Location:      Halbouty 174

Credit Hours:  3 CR

### Instructor Details

Instructor:    David Bapst

Office:        Halbouty 169

E-Mail:        <dwbapst@tamu.edu>

Office Hours:  Mon/Wed: 9:00-10:00 AM, Tue/Thu: 3:40-4:30 PM 

<!--
# Designated Substitute, In Case of Emergency

# Name & Email: Christina Belanger (christina.belanger@tamu.edu)
-->

### Course Description

The course covers scientific programming and statistical methods commonly used in geology and paleontology. Course material will involve applying univariate and multivariate statistical analyses to geological data, and writing short programming scripts for R. Students will gain practical expertise in evaluating statistical approaches and solving methodological obstacles.

<!--
#  Provide a course description that closely follows the catalog description for the course.
-->

### Course Prerequisites

None.

<!--
#  Include a list of course prerequisites (must match Catalog). If no prerequisites, state “None.”
-->

### Special Course Designation

None.

<!--
#  Specify if the course has one (or more) of the following special course designations: core curriculum (CORE), international and cultural diversity (ICD), cultural discourse (CD), writing intensive (W), communication intensive (C), cross-listed, or stacked.

#  Include other information as required for the special course designation (e.g., a W course syllabus must specify the student must pass the writing components to earn a grade in the course, a CORE course must include information about the foundational component area to which it belongs, a stacked course must clearly indicate additional work for graduate students, etc.).
-->

### Course Learning Outcomes

Graduate students who complete this course should be able to:

 * Manipulate relevant datasets of environmental, historical and spatial observations in a programmatic environment, including loading, cleaning and transforming the data.
 
 * Combine functions for loading, manipulating and analyzing datasets into a project workflow.

 * Troubleshoot error messages and other problems with their code.

 * Identify appropriate analyses for a given question or hypothesis, with a particular dataset.

 * Apply familiar statistical tests to new datasets.

 * Teach themselves an unfamiliar statistical test to apply to their own data.

 * Interpret statistical results in terms of a given study system, and suggest possible future directions.

 * Intuit possible biases or issues with an analytical approach.

 * Devise novel analytical approaches when necessary, using statistical theory, simulations, etc.

<!--
#  List one or more learning outcomes for the course.

#  A learning outcome is a statement regarding what the student will know or be able to do upon successfully completing the course. It must be both observable and measureable. The outcomes may include competencies developed in the course. Additional assistance with learning outcomes is available through the Center for Teaching Excellence and the Office of Institutional Assessment.
-->

### Textbook and/or Resource Materials

Students need access to their own computer, on which they should have the R interpreter (install from CRAN: https://cran.r-project.org/), the integrated development environment (IDE) Rstudio (install from the Rstudio website, https://www.rstudio.com/products/rstudio/download/#download), and a spreadsheet program (such as Microsoft Excel). Both R and RStudio are available for free, and LibreOffice Calc is a free spreadsheet program. 

This class has no mandatory textbook, but some optional suggestions for reference are:

 * **Davis, 2003.** Statistics and Data Analysis in Geology. Detailed discussions of many methods we’ll apply, including multivariate methods, with application to geology, despite some aged content.

 * **McKillup and Dyar, 2010.** Geostatistics Explained. Clear explanations on how probability and statistics work, and about geospatial and temporal analyses specialized to geosciences. 

 * **Hammer and Harper, 2006.** Paleontological Data Analysis. A ‘cookbook’ reference to data analysis methods, with introductory summaries on many methods, but without details of how methods work. This book is specialized for paleontology, but will be useful to others as well.

<!--
# Specify the textbook and other resource materials that are required, recommended, and/or optional for the course. If no textbook or other resource materials, state “None.”

#  The syllabus should not promote any one vendor of course materials to the students. Instead, the syllabus should encourage students to acquire the “required and recommended” course material from vendors that provide the best value and amenities for their selection.

#  \pagebreak
-->

### Grading Policy

Your final letter grade will be based on the final percentage grade for the course:

|        |  
| -----  |  --------
| **A**  |  90-100%
| **B**  |  80-89% 
| **C**  |  70-79%
| **D**  |  60-69%
| **F**  |  Less than 60%

Your final percentage for the course will be based on:

|                                                |     
| ---------------------------------------------- | ----
| Project Paper                                  | 40%
| Homework Assignments                           | 20%
| Project Presentation: Questions & Data         |  3%
| Project Presentation: Methods                  |  7%
| Final Project Presentation                     | 10%
| Submitting a Draft for the Introduction & Data |  5%
| Submitting a Draft for Introduction & Methods  |  5%
| Submitting an Early Full Draft                 |  5%
| Submitting a Project Pitch                     |  5%


Grades in this class will be based on in-class presentations, participation, a series of individual homework assignments, and a final project. 

#### Homework Assignments

Individual homework exercises will which must be submitted as single-author reports, but students can work on them as a group -- in fact, students are encouraged to discuss the homework with each other and to compare code outside of class. These homework assignments will generally focus on the programming functions and statistical methods we have covered recently in class, applied to a real dataset. While it is important that you learn to program, my main interest is in assessing how well you are interpreting the relationship between questions and the methods we apply, how the dataset can influence this relationship, and how well you can interpret the results and put them into context. Thus, submitted reports should generally be in prose, with complete sentences and standard paragraph structure, just as text would be written in a scientific paper rather than simply a dump of computer code, or copy-pasted blocks of raw output printed to the terminal. Figures should also be properly labeled and understandable to the reader.

<!--
# Participation & Leadership

Students are expected to participate in hands-on, in-class coding exercises throughout the semester, as well as demonstrating leadership in discussions regarding lecture topics and their proposed final project topic. Participation grades will be based on consistently giving end-of-class feedback at the end of live-coding activities (via supplied Post-It Notes), and involvement in class-wide discussions on problems they have encountered in the course of analyses (technical, theoretical, etc).
-->

#### Term Project, Drafts and Final Project Paper

This class requires a project-based term paper, with students proposing a project focused on research question of their own selection from within the earth and environmental sciences. Students are required to locate and obtain an appropriate dataset – perhaps from a publicly-available source, such as supplemental material for an article, or collected as part of their own research, or supplied by their advisor. **Datasets must be large enough and detailed enough to address a worthwhile research question.** Addressing these research questions will require applying various analyses from throughout the course, and possibly beyond the covered course material. 

During Week 2, students must submit a **Project Pitch**, where they briefly describe one or more potential research projects they might persue, and where they would get the data necessary, and the questions that would be addressed. 

Interim drafts of the term paper are due at three points during the semester:

1. The first draft due, the **Introduction and Data Draft**, is expected to contain (at a minimum) the introduction, and a partial Methods section that describes the context and background of the data: where, when, and *how* was the data collected, and also describing any necessary treatments required to further analyze the data. 

2. The second draft, the **Methods Draft** is expected to build off the former draft, but also describe the analytical approaches the student will apply in the Methods section. 

3. The third draft due should be a relatively complete **Early Full Draft**, adding results, discussion and any necessary figures or tables. 

Each of these three interim drafts **should have** proper in-text citations and formatted references, include a file containing the current data set used for the project, regardless of whether it has been modified since the original data submission. 

Each draft will be graded relative to the final paper rubric, and grades for complete drafts (the third draft submitted should at least be complete, possibly earlier drafts as well) will lock in a students’s scores as a ‘minimum’ grade, upon which students can only improve with successive submissions including the submission fourth and final draft, the finished **Project Paper**. The grade on that final term paper accounts for 40% of your grade. 

See the project papers's grading rubric for details.

#### Expected Structure for the Term Paper

The length of your final paper will depends on how much you have to say to build an efficient, compelling investigation of your question. This final paper should be formatted like a scholarly manuscript, covering the methods, and results of their project. A complete paper draft will have the following required sections:

 * **Abstract  (REQUIRED)** - A concise, 1 paragraph summary of your study (e.g. questions, data, methods, results).

 * **Introduction  (REQUIRED)** - Provide scientific context for your research question and background a reader would need to understand your study system and the importance of answering your research question. State your questions clearly and introduce how you will investigate them.
 
 * **Methods  (REQUIRED)** - A complete description of the data and analyses you use, with justifications for why you chose those specific methods. Include references that support your decisions.

 * **Results  (REQUIRED)** - A report of the results of your analyses, including reporting all necessary statistical values, and necessary supporting figures and tables. Interpretation of results should be minimized.

 * **Discussion  (REQUIRED)** - An interpretation of your results in the context of the hypothesis you set out to test with reference to the published results of other workers. Address any analytical challenges, alternative interpretations, related your findings to the work of others, implications of your results to the field, and suggestions for future work that could improve your ability to answer your research questions.

 * **Conclusions (OPTIONAL)** - A concise summary of the “take-home” results, interpretations, and implications of your research. Similar to the abstract, but does not restate the study’s setup.

 * **References  (REQUIRED)** - Choose a consistent journal format. If uncertain which to use, use Paleobiology style, as it the instructor's favorite.

 * **Data Appendix  (REQUIRED)** - A file or table that contains all data you used for your paper. You must submit a data appendix with the draft of your Introduction and Methods draft, but you should update this appendix as you revise or add to your data over the course.


#### Project Presentations

In week 3, students will take turns introducing the rest of the class to the data and questions they are planning on addressing in the term project. This presentation does not require slides or graphics (although you can use them if you want), and should be less than 5 minutes in duration. 

Similarly, in week 10, students will again present to the class their project, covering again the questions motivating the research, the nature of the dataset, and which methods they are planning to apply, or have already applied, to the dataset. Students should particularly focus on any difficulties they've encountered, or confusion they have about which methods to apply. Again, slides or graphics are not necessary, and the presentation should be kept brief, preferably under 5-8 minutes.

In the last week of the course, students will be asked to prepare a more detailed presentation as an endcap to the research project for the semester, to give in class as a 10-15 minute presentation. Slides, figures and any other graphic aids are recommended. Students are expect to re-introduce the rest of the class to the motivation behind their analyses, the data they used, the methods they applied and why they chose those methods, and what the results can tell us about in the context of the system.

For all the above presentations, students in the audience will actively participate by posing questions (for the live presentations), as well as providing written feedback about each other's presentations, which I will pass in an anonymized form to the presenter. Giving peer feedback, particularly on the final presentation, is a component of the Project Presentation grade.




<!--
# * Define a grading scale for the assignment of a letter grade (A through F) or the criteria for assigning S/U grades as appropriate.
# * Describe the graded items for the course. 
# * Indicate weights as applicable for grade items included in calculating the course grade (e.g., exams, laboratory assignments, field student work, projects, papers, homework, class attendance, participation, and other graded activities).

# **Graded Class Participation** – If class participation constitutes more than 10% of grade, the syllabus should explicitly define and outline how the participation grade is determined based on a well-defined rubric (see (Student Rule 10)[]). 

# **Graded Attendance** – If attendance is a graded item, the syllabus should state how the faculty member will collect and evaluate attendance. 

# **Grades for Stacked Course** – If the course is a stacked course that uses a single, combined syllabus for the undergraduate and graduate courses, the syllabus must clearly specify additional work required for graduate students. (See Policy for Stacked Courses.)

# **Grading Policy Changes** – Faculty must provide grading policies to students by the first class period. As such, faculty cannot change the course grading policy after the second class session. (See Student Rule 10.) 
-->

### Late Work Policy

Late work is discouraged, but will be accepted with a penalty relative to how late the submission is, depending on the assignment and reason given for the late submission. Work submitted late due to an excused absence is not considered late work, and is exempt from the late work policy.

<!--
# Indicate whether or not the faculty member will accept late work. 
# Identify any associated penalty if the faculty member accepts late work for evaluation. 

# The late work policy should define what constitutes late work (e.g., submitting a deliverable after the established deadline). Work submitted by a student as makeup work for an excused absence is not considered late work and is exempted from the late work policy. (See Student Rule 7.)
-->

### Course Schedule

|**Week** |    |**Date** | **Topics Covered**                                                | **Assignments**                         |
|:-------:|:--:|:-------:| ----------------------------------------------------------------- | ----------------------------------------- |
|      1  | Tu | Aug  24 | Course Introduction, Questions and Methods in Science             | |
|         | Th | Aug  26 | Structure of Earth & Environmental Datasets                       | |
|      2  | Tu | Aug  29 |  Using the R Terminal & RStudio; Object Types in R: Vectors, Matrices, Factors, Lists  | Install R and RStudio Before Class  |                                  
|         | Th | Aug  31 | Logicals, Subsetting Vectors and Matrices, and Scatterplots       | **Graduate Student Project Ideas Due**    |
|      3  | Tu | Sept 5  | Loading Datafiles, Using Scripts and If-Else Controls | **Assignment Begins:** *Load This File*   | 
|         | Th | Sept 7  | For Loops, Functions, **Grad Students Present Proposed Term Project Ideas**   | |
|      4  | Tu | Sept 12 | Histograms in R, Probability, Sampling, Odds & Venn Diagrams    | **Assignment Due:** *Load This File*      |
|         | Th | Sept 14 | A Toolbox of Useful Probability Distributions & Summary Statistics | |
|      5  | Tu | Sept 19 | Basic Statistical Measures and Visualizing Observable Data with Boxplots in R | **Assignment Begins:** Ostracod Size Differences |
|         | Th | Sept 21 | Deterministic Models vs Stochastic Simulations | |
|      6  | Tu | Sept 26 | The Basic Recipe of Frequentist Tests | **Assignment Due:** Ostracod Size Differences |
|         | Th | Sept 28 | Bootstrapping, Jack-Knifing and Rarefaction for Dealing with Odd Data | **Assignment Begins:** Modeling Earthquakes with Waiting Time Distributions |
|      7  | Tu | Oct   3 | Parametric vs. Non-Parametric; The Dangers of Multiple Comparisons, Spurious Correlations, and Non-Independence ||
|         | Th | Oct   5 | Statistical Tests for Univariate Datasets: T-Tests, F-Tests, ANOVA (1-Way and 2-Way)  | **Assignment Due:** Modeling Earthquakes with Waiting Time Distributions |
|      8  | Tu | Oct  10 | FALL BREAK - NO CLASS | |
|         | Th | Oct  12 | Statistical Tests for Comparing Categorical Data: Binomial Test and the *Very* Useful Chi-Square Test | **Graduate Students: Draft of Introduction and Data Due** |
|      9  | Tu | Oct  17 | Statistical Methods for Bivariate Data: Correlations and Linear Regression  | **Assignment Begins:** Disentangling Measurement Methods in Digital Field Geology | 
|         | Th | Oct  19 | Logistic Regression, Multiple Regression : Too Many Models |  |
|     10  | Tu | Oct  24 | Frequentist Statistics vs Maximum Likelihood and Other Inferential Schools of Thought | **Assignment Due:** Disentangling Measurement Methods in Digital Field Geology |
|         | Th | Oct  26 | Information Criteria, Model Selection Methods and Stepwise Regression in Multiple Regression | |
|     11  | Tu | Oct  31 | **Graduate Students Present Progress Reports on Selecting Analytical Methods** |  |
|         | Th | Nov   2 | Step-Wise Multiple Regression Model Selection with AIC |   **Methods Draft Due**; **Assignment Begins:** Predicting Groundwater Quality from Geochemical Data | |
|     12  | Tu | Nov   7 |  Distance Matrices and Cluster Analyses for Multivariate Data  | |
|         | Th | Nov   9 | Decomposition of Complex Datasets with Principle Components Analysis | **Assignment Due:** Predicting Groundwater Quality from Geochemical Data |
|     13  | Tu | Nov  14 | Trends and Autocorrelation in  Time-Series | **Full Draft Due** |
|         | Th | Nov  16 | Multivariate Data Wrap-Up | | 
|     14  | Tu | Nov  21 | *Troubleshooting Day* | |
|         | Th | Nov  23 | Holiday - NO CLASS ||
|     15  | Tu | Nov  28 | *Troubleshooting Day* | |
|         | Th | Nov  10 |  **Final Presentations (All Students)** , Course Feedback |   |
|         |    |         | ***Final Draft Due on assigned Final Exam day: December 12th*** 


This course will proceed at the pace at which students can keep up with the material and in-class activities. If we need to circle back on something a few times so a concept is understood, we will do that. Troubleshooting days will be used as 'catch up days' may be used if we are behind on the lecture material but will otherwise be used to check in with students about their final projects and tackle issue that they are having difficulty with solving on their own.

<!--
# |         | F | Nov  25 | *Troubleshooting Day* |  |

# * Include a list of topics, calendar of activities, major assignment dates, and exam dates. 

# The course schedule must include lab hours in the calendar of activities. The course schedule must include dates of major exams and assignments. Dates for exams and assignments should not be changed without written notification to all students in the course (notice via email or learning management system is acceptable). 

# **Traditionally Delivered Course** – The calendar must include the number of weeks that correspond to the traditionally delivered course semester (e.g., Fall/Spring = 15 weeks; Summer = 5 or 10 weeks as appropriate).

# **Non-Traditionally Delivered Course** – The weeks on the calendar of activities for a non-traditional syllabus will vary according to need. Faculty members in departmental units will determine whether the contact hours for a non-traditional course are appropriate for and equivalent to a traditional course. (See University Rule 11.03.99.M1.)
-->


### Optional Course Information Items

* **Writing Support** – The [University Writing Center (UWC)](http://writingcenter.tamu.edu/) has trained peer consultants available to work with you on any kind of writing or speaking project, including research papers, lab reports, application essays, or creative writing, and at any stage of your process, whether you're deciding on a topic or reviewing your final draft. You can also get help with public speaking, presentations, and group projects. We can work with you in person at our Evans or BLCC locations or via Zoom or email. To schedule an appointment or to view our handouts, videos, or interactive learning modules, visit writingcenter.tamu.edu. If you have questions, need help making an appointment, or encounter difficulty accessing our services, call 979-458-1455 or [email](uwc@tamu.edu)].

* **Technology Support** – A great deal of this course involves using the programming language R on a computer. If you have technology issues with installing or running this software, please feel free to email the instructors so they can help you troubleshoot. A quicker and generally effective method is to take whatever message or warning that you've received, and try searching for solutions online using a search engine. For issues with University infrastructure, like the campus wifi or Canvas, you should contact [TAMU IT Help Desk Central](https://it.tamu.edu/help/) via email, virtual chat, phone, etc.

* **Student Resources** – A variety of student resources focused on health and safety are available to you should you need them, listed at the ECCB program's  [Student Resources page](https://eccb.tamu.edu/student-resources/).


<!--
# * **Learning Resources** – 

# Consider adding the following additional information items to the course syllabus when appropriate. 

# * **Technology Support** – Provide appropriate technical support information to inform students who to contact if they encounter technical difficulties (e.g., direct technical questions to the course teaching assistant; contact the vendor; etc.). Technical support information should include information such as who to contact, how to contact that resource, hours of availability, etc. 

# * **Learning Resources** – Provide information regarding available learning resources such as supplemental instruction or tutoring when appropriate (e.g., information about the University Writing Center for a W/C designated course or related LinkedIn Learning modules appropriate for the course topic). The Study Hub website lists many on-campus learning resources to support students in achieving academic excellence.
-->

## University Policies

<!--
# This section outlines the university level policies that must be included in each course syllabus. The TAMU Faculty Senate established the wording of these policies. 

# NOTE: Faculty members should not change the written statements. A faculty member may add separate paragraphs if additional information is needed. 
-->

### Attendance Policy

The university views class attendance and participation as an individual student responsibility. Students are expected to attend class and to complete all assignments. 

Please refer to [Student Rule 7](https://student-rules.tamu.edu/rule07/) in its entirety for information about excused absences, including definitions, and related documentation and timelines.

### Makeup Work Policy

Students will be excused from attending class on the day of a graded activity or when attendance contributes to a student’s grade, for the reasons stated in [Student Rule 7](https://student-rules.tamu.edu/rule07/), or other reason deemed appropriate by the instructor. 

Please refer to [Student Rule 7](https://student-rules.tamu.edu/rule07/) in its entirety for information about makeup work, including definitions, and related documentation and timelines.

"Absences related to Title IX of the Education Amendments of 1972 may necessitate a period of more than 30 days for make-up work, and the timeframe for make-up work should be agreed upon by the student and instructor” ([Student Rule 7](https://student-rules.tamu.edu/rule07/), Section 7.4.1).

"The instructor is under no obligation to provide an opportunity for the student to make up work missed because of an unexcused absence” ([Student Rule 7](https://student-rules.tamu.edu/rule07/), Section 7.4.2).

Students who request an excused absence are expected to uphold the Aggie Honor Code and Student Conduct Code. (See [Student Rule 24](https://student-rules.tamu.edu/rule24/).)

### Academic Integrity Statement and Policy

> ***“An Aggie does not lie, cheat or steal, or tolerate those who do.”***

*“Texas A&M University students are responsible for authenticating all work submitted to an instructor. If asked, students must be able to produce proof that the item submitted is indeed the work of that student. Students must keep appropriate records at all times. The inability to authenticate one’s work, should the instructor request it, may be sufficient grounds to initiate an academic misconduct case”* (Section 20.1.2.3, [Student Rule 20](https://aggiehonor.tamu.edu/Rules-and-Procedures/Rules/Honor-System-Rules)).

You can learn more about the Aggie Honor System Office Rules and Procedures, academic integrity, and your rights and responsibilities at [aggiehonor.tamu.edu](https://aggiehonor.tamu.edu/).

<!--
# NOTE: Faculty associated with the main campus in College Station should use this Academic Integrity Statement and Policy. Faculty not on the main campus should use the appropriate language and location at their site.
-->

### Americans with Disabilities Act (ADA) Policy

Texas A&M University is committed to providing equitable access to learning opportunities for all students. If you experience barriers to your education due to a disability or think you may have a disability, please contact the Disability Resources office on your campus (resources listed below) Disabilities may include, but are not limited to attentional, learning, mental health, sensory, physical, or chronic health conditions. All students are encouraged to discuss their disability related needs with Disability Resources and their instructors as soon as possible.

Disability Resources is located in the Student Services Building or at (979) 845-1637 or visit [disability.tamu.edu](https://disability.tamu.edu/).

<!--
# NOTE: Faculty associated with the main campus in College Station should use this Americans with Disabilities Act Policy statement. Faculty not on the main campus should use the appropriate language and location at their site.
-->

### Title IX and Statement on Limits to Confidentiality

Texas A&M University is committed to fostering a learning environment that is safe and productive for all. University policies and federal and state laws prohibit gender-based discrimination and sexual harassment, including sexual assault, sexual exploitation, domestic violence, dating violence, and stalking.

With the exception of some medical and mental health providers, all university employees (including full and part-time faculty, staff, paid graduate assistants, student workers, etc.) are Mandatory Reporters and must report to the Title IX Office if the employee experiences, observes, or becomes aware of an incident that meets the following conditions (see [University Rule 08.01.01.M1](https://rules-saps.tamu.edu/PDFs/08.01.01.M1.pdf)):

* The incident is reasonably believed to be discrimination or harassment. 
* The incident is alleged to have been committed by or against a person who, at the time of the incident, was (1) a student enrolled at the University or (2) an employee of the University. 

Mandatory Reporters must file a report regardless of how the information comes to their attention – including but not limited to face-to-face conversations, a written class assignment or paper, class discussion, email, text, or social media post. Although Mandatory Reporters must file a report, in most instances, you will be able to control how the report is handled, including whether or not to pursue a formal investigation. The University’s goal is to make sure you are aware of the range of options available to you and to ensure access to the resources you need.

Students wishing to discuss concerns in a confidential setting are encouraged to make an appointment with [Counseling and Psychological Services](https://caps.tamu.edu/) (CAPS). 

Students can learn more about filing a report, accessing supportive resources, and navigating the Title IX investigation and resolution process on the University’s [Title IX webpage](https://titleix.tamu.edu/).


<!-- 
# NOTE: Faculty associated with the main campus in College Station should use this Title IX and Statement on Limits of Liability. Faculty not on the main campus should use the appropriate language and location at their site.
-->

### Statement on Mental Health and Wellness

Texas A&M University recognizes that mental health and wellness are critical factors that influence a student’s academic success and overall wellbeing. Students are encouraged to engage in healthy self-care by utilizing available resources and services on campus. 
Students who need someone to talk to can contact Counseling & Psychological Services (CAPS) or call the TAMU Helpline (979-845-2700) from 4:00 p.m. to 8:00 a.m. weekdays and 24 hours on weekends. 24-hour emergency help is also available through the National Suicide Prevention Hotline (800-273-8255) or at [suicidepreventionlifeline.org](https://suicidepreventionlifeline.org/). 

<!-- 

## College and Department Policies

# College and departmental units may establish their own policies and minimum syllabus requirements. As long as these policies and requirements do not contradict the university level requirements, colleges and departments can add them in this section.

-->
