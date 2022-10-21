# No Limit Hold'em Hand Analyzer

## This is a work in progress.

## Languages/Software Used:

### R (RStudio)

## Motivation:

### I like playing poker - specifically No Limit Hold'em. I record my games so I can go back, analyze my decisions and improve my game. With this project I hope to exercise my programming skills, create a tool streamlining hand analysis and cement my poker knowledge along the way.

## What I've Got:

### A block of code that generates every possible combination of boards and hole cards for a heads-up hand.

### Functions returning pot odds, implied odds, effective odds, your odds of making a draw and whether a call is justified based on these statistics.

## Current Problems and Potential Improvements

### I originally attempted to generate a dataframe containing every possible combination of hands and boards, which I would then use in a function inputing your hand plus your opponents' hands and returning everyone's odds of winning pre-flop. However, the resulting dataframe was too large for R - the possibilities are in the billions. So, I'll be looking into integrating SQL to work with this much data.

### I also think my current function returning the odds of making your draw may be technically incorrect but practically close enough. To simplify the function I used some logical and statistical sleight of hand and I have yet to check whether it is really equivalent to the true odds.

### I also figure I can combine all of my current functions into one function taking the pot size, my outs, present and future bets plus the current street(preflop, flop, turn, or river) and returning a complete rundown of my odds and whether a call is justified. This shouldn't be too hard so it's next on my list.

