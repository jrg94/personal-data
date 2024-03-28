# Education Data

The files contained in this directory relate to data I've collected
across my career as an educator. All data is anonymized or directly
related to me, which I have released publicly. The remainder of
this file describes the contents of each file.

## Teaching History

The purpose of the [teaching history](teaching-history.csv) file is
to record the courses I've taught over the years. It's also meant
to be a bit of a lookup table for other files, since each class
has a unique ID. The list below details the headers:

- **Section ID**: a unique identifier for that particular course section (e.g., 7382)
- **Year**: the year the course was taught (e.g., 2023, 2024, etc.)
- **Season**: the season in the academic year the course was taught (e.g., Spring, Autumn, Summer)
- **Department**: the department the course is hosted in
- **Course Number**: the department-specific course code
- **Start Time**: the time class starts for the course in 24-hour time
- **End Time**: the time class ends for the course in 24-hour time
- **Building**: the campus building that takes place as a two character code
- **Room Number**: the number of the room in the building where the course is taught
- **Job Title**: the position I held during that semester (e.g., Graduate Teaching Associate, Lecturer, etc.)
- **Role**: the specific role I held during that course (e.g., Instructor of Record, Grader, etc.)

## Grading History

The purpose of the [grading history](grading-history.csv) file is to
record the score for every assignment ever graded. It was initially
created because the exported spreadsheets from the learning management
system leave a lot to be desired. This way, assignments can be treated
like events where future changes don't disrupt analyses. The list below 
details the headers:

- **Section ID**: a unique identifier linking back to a course in [teaching history](teaching-history.csv)
- **Student ID**: a non-unique identifier to distinguish students in a particular class (note: 
  repeat students may not have the same ID)
- **Title**: the name given to a particular assignment
- **Grade**: the grade assessed for a particular assignment
- **Total**: the maximum number of points a student could earn on that assignment

This file is meant to deprecate the current grade files, which will be
removed at a later date.
