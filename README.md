# test-variant-gen

## Description

Roadmap for MVP Test Tool
Status: In Progress
Contributors: Khachik Ashkaryan
Date: Mar 1, 2025
Representative Mission Statement: “Allowing teachers to focus more on education & mentorship and less on assessments and grading” 
Overview
As part of the MVP, we wish to create a python script as a proof of concept that is able to take an existing exam in pdf form, read it into our data base, and use LLM’s in order to leverage its ability to interpret questions, make them more difficult, different, etc..
Goals
Create quick version of MVP as a proof of concept to demonstrate that the idea is doable and to test engagement.

Requirements P0 (These need to happen):
Establish data structure to hold necessary info about tests (document oriented?)
Types of questions: Multiple choice only, NO diagrams. Simple questions with exact answers (math + science)
Read in PDF and accurately turn them into the desired data structure
Leverage chatgpt to interpret the data structure
Make queries to create versions of incoming questions
Create data structure linking test -> version -> answer_key
Read in a PDF that has answers bubbled in (understand which version the test is reading)
Convert data structure to pdf

Requirements P1 (These should happen, but after P0):
Extend types of questions we can read to include diagrams
Turn into answered version of data structure, and compare to answer key
Get student names with grades 
New data structure for student, test, version, grade (essentially)

Requirements P2 (These would be nice to have, but after P1):
Extend types of supported exams to subjective answers (english exams, essay grader)
Extend read in feature to work with free response questions
Update data structure to allow for manual grade change
Create simple UI for teachers to manage their students grades + their own exams

Requirements P3 (These are wishful thinking):
Add ability to not only create versions of exams, but adjust the variance (variability) of exam
*****NEW FEATURE***** Create additional adjuster to update the difficulty of the questions they’re creating

Requirements P4 (These are long term dreams):
Add ability for teachers to make their entire exams through our platform
Pair with LLM to provide recommendations on how to improve questions.
Create answer key without manual input based on best guess (allowing for manual changes)
Add feature to output a test guide for students based on learning material + active test
Notebook LLM here, probably would need to pair the tool with canvas (api exists!!!)
https://canvas.instructure.com/doc/api/ 
Prompt box for teachers to generate test or other study material via prompt w/o interacting w UI
Roadmap for P0
Create data structure for exams (1 day) KA
Make sample exams in this data structure for testing (1 day)
Find some VERY simple PDF exams 
Write script to take pdf of exam and turn it into the date structure (2-3 days)
Update data structure to accommodate versions of exams (0.5 days)
Try to establish connection with Canvas course (2-3 days) AT
This will open up a world of possibilities
Read in exam from canvas into the data structure form we have (1-2 days)
Create fake course + class for testing purposes
Use LLM to create versions of an exam the simplest way (change up a couple numbers) (4-5 days)
Keep answer key for versions of exam as well (2-3 day)
Make data structure and parse it

Inputs:
Exam from manual pdf upload or Canvas connection
Processing:
Parse data into desired structure, create versions, create answer keys for each versions
Outputs:
Multiple versions of the exam + answer key in desired data structure format
In Progress
Kachik
Establishing “Test” data structure to use for version manipulation
Probably should just reuse the same schema as in Canvas
Need some examples



Avedis


Concerns

