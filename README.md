# Training Log 2.0: Guided Program

A guided strength, speed, and arm care program for Valley Baseball. Each player installs it on their own phone; all data stays on that phone.

## Files
- `index.html` is the app.
- `program.js` is the program: phases, sessions, speed work, arm care, and the exercise library with coaching cues. Edit this file to change the program.
- `program.html` is the coach's program overview: every phase and day, both tracks side by side, an exercise index with coaching cues, and print buttons. It reads `program.js`, so it updates when you edit the program.
- `sw.js` makes the app work offline. Change `VERSION` in it (for example `traininglog-v3`) every time you upload a changed file.

## How the program runs
- 9 weeks, 4 sessions per week, 36 sessions in order. Players always get the next session and cannot skip ahead. One program session per day.
- Monday and Wednesday open with speed work. Every session ends with arm care.
- Weights follow the program's RPE rules: move up the smallest step (5 lb, or 2.5 lb on light dumbbells) after completing every rep with the last set at RPE 7 or easier; repeat after coming up short; drop 10% after coming up short twice in a row.
- Beginners are reviewed at the end of each phase. Meeting all four standards unlocks a move to the Experienced track, which a coach approves with the coach code.

## Track links
- Beginner: https://dhanssen-code.github.io/training-log/#t=b
- Experienced: https://dhanssen-code.github.io/training-log/#t=e

A link sets the track only before a player's first session. After that, only Coach tools (in Profile) can change it.

## Team start date
Set `startDate` in `program.js` to the Monday the team begins, for example `startDate: '2027-01-04',`. Leave it as `''` to let each player's schedule start with their first session.
