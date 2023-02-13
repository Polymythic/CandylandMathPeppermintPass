# Overview
Run simulated games to see if its better to take a maximum distance selection strategy, or a minimum move strategy to try to gain the Peppermint Pass shortcut.  

# Introduction
I am a long time boardgamer and was a new father some time ago who wanted to use boardgaming to teach my children useful skills such as taking turns.  Candyland always seemed very limitied because of the simple draw-and-move mechanism.  There was no choice at all, and was pure luck to the end.  

However, in revewing the rules, there was a "draw 2 cards and make a choice" variant.  This introduced a fundamental improvement to the game experience: choosing which move is better.  I though this would at least engage young minds that a double move is better than a single move, and assessing which color would take you further down the track based on your current position.  This required some light level of analysis. 

Finally, something scratched at me as it pertains to using the draw 2 selection and the specific layout of my version of the game (https://candyland.fandom.com/wiki/Candy_Land_(2010)) with the Peppermint Pass.  The Peppermint Pass is a shortcut offered in the 4th square of the game (a blue square) that takes the lucky drawer a whopping 60 squares down the track.  

## The Question - Is there a deeper strategy?
So, would it make sense for a player who did NOT draw the single blue enabling a Peppermint Pass to actually HOLD OUT for that opportunity by selecting a minimum movement, thus maximizing the chance of drawing the Peppermint Pass next turn?  In essence, the payout is so large, move a few spaces as possible to maximize the chance of getting a single blue and a payout of 60.


# Simulation and Rules
Simulate if its more beneficial to take the shortest movement to try to get the Peppermint Pass.  

* IF the minimum mover is forced to move past the shortcut square, they have lost
* IF the minimum mover gets the shortcut square but the max mover has moved further that 60 they have lost
* IF either min or max mover gets the shortcut, they take it and its a win for the miniumum

Note: there are some nuances that may not be implemented such as a max mover falling into licorice and losing a turn, or taking a second shortcut.  Those may be added later to improve the statistics.

# Conclusions
It appears that the min-movement strategy comes out on top 45% of the time for that early game choice.  High risk, high reward I guess.