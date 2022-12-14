# No Limit Hold'em Hand Analyzer

## This is a work in progress.

## Languages/Software Used:

### R (RStudio)

## Background:

- I like playing poker, specifically No Limit Hold'em. I record myself so I can go back, analyze my decisions and improve my game. With this project I hope to exercise my programming skills, create a tool streamlining hand analysis and cement my poker knowledge along the way. Some functions are even convenient enough to consult mid-game and have directly resulted in profitable decisions for me.

## What I've Got:

- Functions taking street(flop, turn), pot size, your outs and bet sizes which returns various odds and whether calling a bet is justified.

- Function taking your hand, the table limit and your stack size which returns your hand's Slansky-Chubukov value and whether it makes sense to get all-in preflop.

## Planned Additions:

- Range Analysis Functions: Construct general fold/call/bet/raise frequences for all hands and then create a function taking an opponent's action on each street as arguments and returning a vector of hands where the combination of observed actions are within some sort of confidence interval of assumed frequencies.

- Equity Calculator: Function returning your win % based on a matchup of hands or your outs.

## Current Challenges:

- Generating all possible combinations of two hands and the board is too large for R. The resulting dataframe is larger than 2.1 billion rows. I anticipate involving SQL in the project to host the data.

- My current formulas for the odds of making your hand based on your outs are inaccurate when it comes to two-card draws like backdoor straights and backdoor flushes, especially when you have BOTH a backdoor straight and a backdoor flush draw. Calculating this as conveniently and accurately as possible is a priority.

