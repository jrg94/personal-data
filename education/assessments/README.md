# Assessment Data

### Assessments

The purpose of the [assessment lookup](assessment-lookup.csv) table is to
provide additional information about each assessment I have ever administered.
The file is setup to be expanded if needed. For now, the headers are as follows:

- **Assessment ID**: a unique identifier for that particular assessment (e.g., 1)
- **Assessment Group ID**: a unique identifier linking back to an assessment group in the [assessment group lookup](assessment-group-lookup.csv) table
- **Assessment Name**: the name of the assessment (e.g., Homework #4)

## Grades

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

## Groups

The purpose of the [assessment group lookup](assessment-group-lookup.csv) table
is to provide additional information about groups that assessments may belong
to. These assessment groups are then used to weight subsets of assessments.
The file is setup to be expanded if needed. For now, the headers are as follows:

- **Assessment Group ID**: a unique identifier for a particular assessment group (e.g., 1)
- **Assessment Group Name**: the name given to the assessment group (e.g., Homeworks)
- **Assessment Group Weight**: the weight given to the assessment group out of 100 (e.g., 25)
