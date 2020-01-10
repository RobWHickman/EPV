---
title: "README"
output: github_document
pagetitle: README
---

<img src = "hex_sticker/HexSticker2.png" align = "right" width = "300"/>

# EPV
R package to implement various Expected Possession Value models

Written by Robert Hickman, October 2019 and January 2020






## What motivates this package

### How do we quantify the effect soccer players have

The motivating idea behind Expected Possession Value models of football events is that each action (or 'event') a player makes has some impact upon the expected final result. The simplest and most dramatic example of this is a spectacular long range drive suddenly changing the score differential. For example:

![James Rodriguez vs. Uruguay](/soccer_gifs/colombia_v_uruguay.gif)

In this example James Rodriguez controls the ball and scores a very low xG chance to give Colombia the lead over Uruguay in the 2014 World Cup Round of 16. If we want to quantify the effect this one movement has had on the game, we can calculate it as the change in score from the event minus the pre-action expected change in score. Let's be charitable and say one out of 10 shots Rodriguez attempts from here would be scored, this resolves to:

xG added: 1 - 0.1 = 0.9

A fairly substantial contribution given the total post-game xG for any side in any football match is likely to be between 0 and 3!

### How do we quantify non-shot events

However, most actions are trying to progress the ball into an area where a better shot can be taken from. When in possession this is done by either passing or carrying/dribbling the ball, for example:

![Robin van Persie vs. Spain](/soccer_gifs/netherland_pass_v_spain.gif)

Or when out of possession, by pressing/tackling the opposition to win the ball back and allow a chain of passes/carries to begin.



## Bibliography
1. [Singh, Introducing Expected Threat (xT), 2019](https://karun.in/blog/expected-threat.html) - the blog post introducing the expected threat (xT) metric and the theory behind it (to be added: Statsbomb conference video)
2. [Hickman, Considering Defensive Risk in Expected Threat Models, 2019]() - My own paper presented at the 2019 Statsbomb conference playing with some ideas around xT (to be added with talk video)
