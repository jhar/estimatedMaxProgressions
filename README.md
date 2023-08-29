# Estimated Max Progressions

An "estimated max" (EM) is a theoretical value for what someone could possibly execute for a one rep max (1RM) on any given strength training exercise given how many reps they can perform at a lighter weight. 1RM and EM are typically only discussed for compound, barbell movements (such as the back squat, bench press, and/or deadlift) where doing such a thing is practical and relatively safe.

This project is a collection of Jupyter notebooks that plot the highest EM that I've achieved during a workout for a particular lift over time.

## Considerations
1. EM formulas are more accurate on sets where someone attempts as many reps as possible (AMRAP) at a given weight, but will underestimate when someone uses the same weight for repeated sets (sets across). In my data, there is a mix of AMRAP sets and sets across, since consistently doing AMRAP sets is physically and neurologically taxing. This typically results in a visible oscillation of values from workout to workout.
2. EM formulas are more accurate on lower rep sets, and less accurate on higher rep sets. It's generally recommended to not use rep counts over 12.
3. There are many different formulas. The EM in my data is simply the mean of 7 different known formulas. This calculation is not included in this repo.
4. If a lift is done with sufficiently high frequency (think daily), then EM will vary wildly. The regression curve through these points won't be a reflection of limit strength, but more a reflection of what is likely to be achieved in a diminished state on a daily basis.
5. Deload workouts are noticeable as striking dips. This is where less weight is intentionally used or fewer reps intentionally performed for the sake of physical or mental recovery.
6. Injury is a confounding factor. In some of the notebooks (particular the ones for low-bar squat variations), you may notice a trend of consistent progress, destabilization, diminishment, and then cessation. I've been forced to cycle through squat variations a few times this year because of the aggravation of pre-existing knee injuries and quad tendonitis.
7. Some lifts are simply less of a priority, and less effort and aggression is put into progressing them.
8. Accomodating resistance (band tension, chains) is not added to weight. Only the weight from the bar and plates is counted. For the banded deadlift with +44 lbs of band tension, this means that 392.5x3 means there is 392.5 lbs of total resistance at the bottom of the range of motion, and 436.5 lbs at the top. How this factors into an EM for a lift performed without accomodating resistance is hard to predict.