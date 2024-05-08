# Lookup Tables

There is a variety of high-level data that I track that can
help with various educational data from evaluations to assessments.
I generically call these lookup tables because they're generally
small and serve to contextualize all other data.

## Courses

The purpose of the courses lookup table is to provide
additional information about each of the courses I teach or have taught.
The file is setup to be expanded if needed. For now, the headers are as
follows:

- **Course ID**: a unique identifier for that particular course (e.g., 1)
- **Course Department**: the department that houses that course (e.g., CSE)
- **Course Number**: the department-specific code for that course (e.g., 2221)
- **Course Name**: the official name of the course (e.g., Software Components)

## Scales

The purposes of the scales lookup table is to provide
Likert scale data that's used in a variety of spaces, such as
SEIs and other feedback surveys. The list below details the
headers:

- **Scale ID**: a unique identifier for each scale element
- **Scale Name**: a scale name (e.g., Agreement, Quality, etc.)
- **Scale Label**: a scale element name (e.g., Strongly Disagree, Poor, etc.)
- **Scale Value**: a scale element value between 1 and 5

## Sections

The purpose of the sections lookup table is to record the course sections 
I've taught over the years. The list below details the headers:

- **Section ID**: a unique identifier for that particular course section (e.g., 7382)
- **Calendar ID**: a unique identifier linking back to a semester
- **Course ID**: a unique identifier linking back to a course
- **Course Type**: the university designated label for the section ID (e.g., Lecture, Lab, etc.)
- **Section Days**: the days a section is taught (e.g., WeFr)
- **Section Start Time**: the time class starts for the course in 24-hour time
- **Section End Time**: the time class ends for the course in 24-hour time
- **Section Building**: the campus building that takes place as a two character code
- **Section Room Number**: the number of the room in the building where the course is taught
- **Educator Title**: the position I held during that semester (e.g., Graduate Teaching Associate, Lecturer, etc.)
- **Educator Role**: the specific role I held during that course (e.g., Instructor of Record, Grader, etc.)

## Semesters

Education data is a bit confusing because it relies on time-series
data that isn't of the normal form. An academic year does not start
in January but rather August. As a result, there needs to be data
table that stores all of this data, among other relevant information
as seen below:

- **Semester ID**: a unique identifier for the semester
- **Semester Year**: a year greater than or equal to 2018
- **Semester Season**: one of the three main academic seasons (i.e., Spring, Summer, and Autumn)
- **Semester Abbreviation**: a shorthand label for the semester
- **Academic Year**: a label meant to group semesters (e.g., 2021-2022)
