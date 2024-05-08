# Assessment Data

The assessments data contains a variety of tables related
to grading and feedback on grading. 

### Assessments

The purpose of the assessment table is to provide additional information about 
each assessment I have ever administered. The file is setup to be expanded if 
needed. For now, the headers are as follows:

- **Assessment ID**: a unique identifier for that particular assessment
- **Assessment Group ID**: a unique identifier linking back to an assessment group
- **Assessment Name**: the name of the assessment (e.g., Homework #4)

## Grades

The purpose of the grades table records the score for every assessment 
ever graded. It was initially created because the exported spreadsheets 
from the learning management system leave a lot to be desired. This way, 
assessments can be treated like events where future changes don't disrupt 
analyses. The list below details the headers:

- **Grade ID**: a unique identifier for each grade
- **Section ID**: a unique identifier linking back to a course section
- **Student ID**: a non-unique identifier to distinguish students in a particular class (note: repeat students may not have the same ID)
- **Assessment ID**: a unique identifier linking back to an assessment
- **Grade**: the grade assessed
- **Total**: the total possible score

## Groups

The purpose of the groups table is to provide additional information about 
groups that assessments may belong to. These assessment groups are then used 
to weight subsets of assessments. The file is setup to be expanded if needed. 
For now, the headers are as follows:

- **Assessment Group ID**: a unique identifier for a particular assessment group (e.g., 1)
- **Assessment Group Name**: the name given to the assessment group (e.g., Homeworks)
- **Assessment Group Weight**: the weight given to the assessment group out of 100 (e.g., 25)

## Reviews

The purpose of the reviews table is to track reviews conducted
by students for a particular assessment. The general purpose of
this data is to track how long students spend on each assessment,
but other interesting data will be included later.

- **Assessment Review ID**: a unique identifier for each review
- **DateTime**: the timestamp of the review
- **Course ID**: the course under review
- **Assessment ID**: the assessment under review
- **Time Taken**: the time spent on the assignment in hours
