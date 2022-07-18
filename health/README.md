# Health Data

The data in this folder is all health related data. Each file is described
in more detail below.

## Fitbit

The fitbit.csv file contains data backed up from my personal fitbit
account. The data is organized into daily rows where dates may
be duplicated. The columns are defined as follows:

- **Date** [Ordinal]: the date of the Fitbit event
- **Steps** [Ratio]: the number of steps completed in a given day
- **Weight** [Ratio]: the weight provided by a scale (may have more than one measure per day)
- **Body Fat %** [Ratio]: the body fat percentage provided by a scale (may have more than one measure per day)

## Weightlifting

The weightlifting.csv file contains data related to weightlifting. The
columns are defined as follows:

- **Date** [Ordinal]: the date of the lift
- **Exercise** [Nominal]: the name of the exercise
- **Muscle Group** [Nominal]: the primary muscle group the exercise targets
- **Sets** [Ratio]: the number of sets completed
- **Reps** [Ratio]: the number of reps in each set
- **Total Reps** [Ratio]: the number of actual reps completed over all sets (may differ from sets times reps)
- **Weight** [Ratio]: the amount of weight lifted (name should give clue about what the weight refers to)
- **Negatives** [Nominal]: TRUE if the exercise was lifted as a negative; FALSE otherwise
- **Difficulty** [Ordinal]: the amount of challenge associated with a given set; possible values include Unknown, Easy, Normal, and Hard
- **Source** [Nominal]: the origin of the data (e.g., paper tracking, app tracking, etc.)
