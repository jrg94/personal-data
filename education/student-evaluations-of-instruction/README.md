# Student Evaluation of Instruction Data

Student Evaluations of Instruction, or SEIs, are surveys
that students complete at the end of each semester for
each of their courses. 

To organize this data, I have placed all of the data in a
series of related files as follows:

## Cohort Scores

When you receive your SEIs, your scores are compared against
various cohorts, such as other courses in your department, your 
college, and your university. The cohort-related data does not
differ from section to section, for obvious reasons, so it's
stored here by semester. The list below details the following
headers:

- **Cohort Score ID**: a unique identifier for each cohort score
- **Semester ID**: a unique identifier linking back to a semester in the academic calendar
- **Question ID**: a unique identifier linking back to an SEI question
- **Cohort**: a cohort (e.g., Department, College, or University)
- **Mean**: an average score between 1 and 5
- **Standard Deviation**: a standard deviation 

## Comments

With each SEI report, there are a series of comments attached.
To track those comments, a separate table was made with the following
headers:

- **SEI Comment ID**: a unique identifier for each comment
- **Report ID**: a unique identifier linking back to an SEI report
- **Comment**: a comment

## Instructor Distributions

With each SEI report, there is per-question breakdown of the
Likert scale distributions. This document is a bit of a work-in-progress
because there is just so much data to enter. That said, I hope one
day to be able to display these distributions. The list below
details the following headers:

- **SEI Instructor Distribution ID**: a unique identifier for each distribution element
- **SEI Report ID**: a unique identifier linking back to an SEI report
- **SEI Question ID**: a unique identifier linking back to an SEI question
- **Scale ID**: a unique identifier linking back to a particular Likert scale label
- **Response Percentage**: a percentage between 0 and 100

## Instructor Scores

With each detailed SEI report, instructor scores are provided with
additional context. For example, in addition to the same means and
standard deviations that you get with each cohort, you also get
the number of responses for each question. This data was separated from
the cohort data because I teach multiple classes a semester, so
there wasn't a way to easily include both sets of data in the same table.
The list below details the following headers:

- **SEI Instructor Score ID**: a unique identifer for each instructor score
- **SEI Report ID**: a unique identifier linking back to an SEI report
- **SEI Question ID**: a unique identifier linking back to an SEI question
- **Response Count**: a number of respondents which is greater than or equal to zero
- **Mean**: an average score between 1 and 5
- **Standard Deviation**: a standard deviation 

## Questions

Each SEI asks the same 10 questions, which are stored in this table.
The list below details the following headers:

- **SEI Question ID**: a unique identifier for each question
- **SEI Question**: a question in plain text
- **SEI Question Group**: a group name in plain text

## Reports

Every semester, I receive a report for each of the classes I teach.
The purpose of this table is basically to detail high-level
information about those reports, such as how many students responded
to the SEI, how many were invited, and the ratio of responses to
invites.

- **SEI Report ID**: a unique identifier for each SEI report
- **Section ID**: a unique identifier linking the SEI report to a course section
- **Responded**: a number of respondents greater than or equal to zero
- **Invited**: a number of students invited to complete the SEI
- **Response Ration**: a ratio of responses to invites between 0 and 100
