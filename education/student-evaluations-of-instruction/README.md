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

- **Calendar ID**: a unique identifier linking back to a semester in the academic calendar
- **Question ID**: a unique identifier linking back to an SEI question
- **Cohort**: a cohort (e.g., Department, College, or University)
- **Mean**: an average score between 1 and 5
- **Standard Deviation**: a standard deviation 

## Comments

With each SEI report, there are a series of comments attached.
To track those comments, a separate table was made with the following
headers:

- **Report ID**: a unique identifier linking back to an SEI report
- **Comment**: a comment

## Instructor Scores

With each detailed SEI report, instructor scores are provided with
additional context. For example, in addition to the same means and
standard deviations that you get with each cohort, you also get
the distribution of responses for each question.

## Questions

## Reports
