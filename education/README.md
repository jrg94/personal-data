# Education Data

The files contained in this directory relate to data I've collected
across my career as an educator. All data is anonymized or directly
related to me, which I have released publicly. The remainder of
this file describes the contents of each file.

## Historical Records

There are a variety of historical records that I maintain. These
include all of the important data that I track over time.
Each historical record is listed in alphabetical order by
its file name. 

### Grading History

The purpose of the [grading history](grading-history.csv) file is to
record the score for every assessment ever graded. It was initially
created because the exported spreadsheets from the learning management
system leave a lot to be desired. This way, assessments can be treated
like events where future changes don't disrupt analyses. The list below 
details the headers:

- **Section ID**: a unique identifier linking back to a course in [teaching history](teaching-history.csv)
- **Student ID**: a non-unique identifier to distinguish students in a particular class (note: 
  repeat students may not have the same ID)
- **Assessment ID**: a unique identifier linking back to an assessment in the [assessment lookup](assessment-lookup.csv) table
- **Grade**: the grade assessed for that particular assessment
- **Total**: the maximum number of points a student could earn on that assessment

### SEI Comments History

The purpose of the [SEI comments history](sei-comments-history.csv) file is to track
all of the comments I have ever received from students in the SEIs. The list
below details the headers:

- **Section ID**: a unique identifier linking back to a course in [teaching history](teaching-history.csv)
- **Comment**: a comment made by a previous student

### SEI Ratings History

The purpose of the [SEI ratings history](sei-ratings-history.csv) file is to track
all of the student evaluation of instruction metrics. The list
below details the headers:

- **Section ID**: a unique identifier linking back to a course in [teaching history](teaching-history.csv)
- **Question ID**: a unique identifier linking back to a question in [SEI questions](sei-questions-lookup.csv)
- **Group**: the group to which the mean result belongs to (e.g., Instructor, University, Department, or College)
- **Mean**: the mean rating out of 5 for that particular question
- **Standard Deviation**: the standard deviation of the ratings for that particular question

Note: a lot of data is duplicated in this CSV. When I teach three times a semester, I am going
to have the same College, University, and Department metrics. Rather than only list them under
one section, I duplicated them to save myself headache later. 

### Teaching History

The purpose of the [teaching history](teaching-history.csv) file is
to record the courses I've taught over the years. It's also meant
to be a bit of a lookup table for other files, since each class
has a unique ID. The list below details the headers:

- **Section ID**: a unique identifier for that particular course section (e.g., 7382)
- **Year**: the year the course was taught (e.g., 2023, 2024, etc.)
- **Season**: the season in the academic year the course was taught (e.g., Spring, Autumn, Summer)
- **Department**: the department the course is hosted in
- **Course Number**: the department-specific course code
- **Course Type**: the university designated label for the section ID (e.g., Lecture, Lab, etc.)
- **Start Time**: the time class starts for the course in 24-hour time
- **End Time**: the time class ends for the course in 24-hour time
- **Building**: the campus building that takes place as a two character code
- **Room Number**: the number of the room in the building where the course is taught
- **Job Title**: the position I held during that semester (e.g., Graduate Teaching Associate, Lecturer, etc.)
- **Role**: the specific role I held during that course (e.g., Instructor of Record, Grader, etc.)

## Lookup Tables

In addition to the historical records, I also maintain a variety
of lookup tables that exist to eliminate some of the clutter from
the tables listed above. 

### Assessment Group Lookup

The purpose of the [assessment group lookup](assessment-group-lookup.csv) table
is to provide additional information about groups that assessments may belong
to. These assessment groups are then used to weight subsets of assessments.
The file is setup to be expanded if needed. For now, the headers are as follows:

- **Assessment Group ID**: a unique identifier for a particular assessment group (e.g., 1)
- **Assessment Group Name**: the name given to the assessment group (e.g., Homeworks)
- **Assessment Group Weight**: the weight given to the assessment group out of 100 (e.g., 25)

### Assessment Lookup

The purpose of the [assessment lookup](assessment-lookup.csv) table is to
provide additional information about each assessment I have ever administered.
The file is setup to be expanded if needed. For now, the headers are as follows:

- **Assessment ID**: a unique identifier for that particular assessment (e.g., 1)
- **Assessment Group ID**: a unique identifier linking back to an assessment group in the [assessment group lookup](assessment-group-lookup.csv) table
- **Assessment Name**: the name of the assessment (e.g., Homework #4)

### Course Lookup

The purpose of the [course lookup](course-lookup.csv) table is to provide
additional information about each of the courses I teach or have taught.
The file is setup to be expanded if needed. For now, the headers are as
follows:

- **Course ID**: a unique identifier for that particular course (e.g., 1)
- **Course Department**: the department that houses that course (e.g., CSE)
- **Course Number**: the department-specific code for that course (e.g., 2221)
- **Course Name**: the official name of the course (e.g., Software Components)

### SEI Questions Lookup

The purpose of the [SEI questions lookup](sei-questions-lookup.csv) file is to define the 10 questions
used in every student evaluation of instruction. The file is setup to be
expanded if needed. For now, the headers are as follows:

- **Question ID**: a unique identifier for the question
- **Question**: the question description
- **Scale**: the max scale value on a Likert scale (e.g., 3, 5, 7, etc.)
