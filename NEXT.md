# Next action

One concrete action per track. Do the one matching tonight's slot, then rewrite this file
before stopping.

## bottom-up
Open `probability-mit-john-tsitsiklis/Assignments/A3.pdf`. Check whether it's already solved.
If blank: solve it. If solved: open `Lectures/M03: continuous random variable.pdf`, review it,
then find and watch MIT OCW 6.041 Lecture 4 (Discrete Random Variables II) on the syllabus page
linked in `curriculum.md`, and take notes into a new `bottom-up/notes/M04.md`.

## top-down
Create `top-down/units/01-heart-rate-distribution/notebook.ipynb`. Use the `mcp__coros__*`
tools (in the root KnowledgeNexus session, not from inside this repo) to pull resting HR and
HRV for the last ~90 days via `queryDailyHealthData` / `querySleepHrv`. Plot a histogram of
resting HR. That's the whole first session — don't fit a distribution yet, just look at the
shape of the data.
