---
title: "dopamine meets reinforcement learning"
date: 2026-08-11T15:34:30-04:00
categories:
  - Books
---
Minsky was the first to build a reinforcement learning algorithm. He did that with the same idea as Thorndike's maze (see below) — an algorithm learning through trial and error. Despite it being a great idea, it didn't end up working well, because the AI would get a reward only at the end of the game, when it responded correctly. That didn't help, since it wasn't clear to the AI which move it was being rewarded for — that is, which move was good and helped it win the game. That is why Minsky proposed the temporal credit assignment problem — assigning credit across time. Back then, that idea was left unresolved for decades, until a man named Richard Sutton proposed a new strategy for solving the temporal credit assignment problem.

His idea was to reinforce behaviors using predicted rewards, meaning that the AI receives a reward when it thinks it is winning, instead of only when it actually wins. There were two components: the actor and the critic. The critic predicts the likelihood of winning, so it signals whether a move is good or bad, whereas the actor is the one that takes the action and gets the reward (or not) depending on whether the critic thinks that the actor's move increased the likelihood of winning. In this way, the AI system learns along the way instead of having to wait until the end of the game. The actor and the critic depend on each other, and they both learn over time. He called this idea temporal difference (TD) learning — the actor learning through the temporal difference in the predicted reward from one moment to the next. 

At the same time, a physicist named Tesauro was working on getting AI systems to play backgammon. He was open to Sutton's idea of letting a system teach itself from its own predictions. The system was called TD-Gammon, and it learned through trial and error, showing strong performance.

After the success of proving that his simulations worked also in real life, Sutton still hoped there was a connection between his idea and the brain. Researchers suspected it had something to do with dopamine, often thought of as the brain's pleasure signal — which, it turns out, is not the case. Dopamine doesn't produce pleasure. The German neuroscientist Wolfram Schultz explained this in more detail and was the first to do so, in the 1980s.

He showed that dopamine neurons initially responded to the reward itself, but after a few trials, they stopped responding to the reward and instead responded only to the predicted cue. So dopamine activity increases for an unexpected reward, or when predicting a reward, and decreases when a reward is expected but not received. Shocking!

A decade later, Dayan and Montague found that Schultz's findings aligned with Sutton's theory. Dopamine neurons in Schultz's monkeys got excited by predictive cues because these cues led to an increase in predicted future rewards; dopamine neurons were unaffected by the delivery of an expected reward because there was no change in predicted future rewards; and dopamine-neuron activity decreased when expected rewards were withheld, because there was a decrease in predicted future rewards.

All of this is to say that dopamine is not a signal for reward but for reinforcement, and that AI models, just like animals, learn best not from being told the answer, but from trial and error.

_____________________________________     
Thorndike's puzzle box: the scientist put animals in a box and let them figure out how to open the door. Once the door was opened, the animal would get a reward (food). He wouldn't tell them what to do but through trial and error the animals learnt that themselves. He reported their behaviour for each trial and found out that after several trials they were able to find the way out quicker. 


P.S. Using em dashes without AI because I love 'em.

<small> Reference: <small/> 
<small> A Brief History of Intelligence - Max Bennett <small/> 
