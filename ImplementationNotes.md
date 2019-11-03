# Implementation Notes

## Bug Fixes

### Reset button does not restore money (high)

Hitting (RESET) after allocating food points de-allocates them but does not reset money to week-start value. Need to implement storage of the money value at the start of each week to allow for mid-allocation reset, and commit change on (Complete Week). 

### Putting negative numbers into (Pay Off Debt) increases debt and money

Unsure if bug or just poorly-afforded feature. Maybe we should make that bucket two-way?

## Features to Add

### Implement NL health qualifiers (low)

Implement word-based health (like with prospects)

### Recurring/Singular  Events (medium)

One-time or recurring events (not randomly allocated as previous idea), such as rent payments or project due dates.

- Implemented as functions of the Week counter, modifiers on multipliers

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

