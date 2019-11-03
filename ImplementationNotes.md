# Implementation Notes

## Bug Fixes

### Putting negative numbers into (Pay Off Debt) increases debt and money (low)

Unsure if bug or just poorly-afforded feature. Maybe we should make that bucket two-way? Also breaks sometimes.

## Features to Add

### Implement random/recurring events (medium)

Using RND of modulo, add occasional positive and negative events. 

### Implement performance effects on prospects (low)

Should prospects be affected by low performance / should prospects be able to go down?

### Energy (high)

Classwork, Exercise, Work should consume energy points as well as time. Maybe 8?

## Design Fixes

### Too Harsh (high)

Drop in performance is too severe week-to-week currently, drop in health feels about right. 

### Time (low)

Time points modified down to 18 -- watch this value in future implementation fixes. 

- 32 possible total allocated points each week, 18 is more than half but not enough to max out 3/4 tasks
- Forces greater choice for week-to-week prioritization

### Money (low)

Money modified down to $5000 -- track this value in testing

### Weeks (low)

Weeks at 50 to graduate -- is this too many? Track in testing. 

