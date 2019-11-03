# Implementation Notes

## Bug Fixes

### Putting negative numbers into (Pay Off Debt) increases debt and money (low)

Unsure if bug or just poorly-afforded feature. Maybe we should make that bucket two-way? Also breaks sometimes.

## Features to Add

### Implement failure conditions (high)

When health hits 0, or performance hits F, lose.

- "You have died of dysentery!"
- "You have failed; MJ is very disappointed in you."
- "You have graduated with %prospects% prospects! You'll find a way to pay off that %debt% debt!"

### Implement performance effects on prospects (low)

Should prospects be affected by low performance / should prospects be able to go down?

### Implement NL health qualifiers (low)

Implement word-based health (like with prospects)

### Recurring/Singular  Events (medium)

One-time or recurring events (not randomly allocated as previous idea), such as rent payments or project due dates. Implemented as functions of the Week counter, modifiers on multipliers

- Rent -- every four weeks additional expenses
- Exams/projects -- every ~6 weeks more classwork is required

### Energy (high)

Classwork, Exercise, Work should consume energy points as well as time. Maybe 8?

### Rent (medium)

Every four weeks, rent should be due, affecting money -- implement as recurring event

## Design Fixes

### Too Harsh (high)

Drop in performance is too severe week-to-week currently, drop in health feels about right. 

### Time

Time points modified down to 18 -- watch this value in future implementation fixes. 

- 32 possible total allocated points each week, 18 is more than half but not enough to max out 3/4 tasks
- Forces greater choice for week-to-week prioritization

### Money (high)

Too much initial money -- not enough motivation to Work. Half or less current starting value.

