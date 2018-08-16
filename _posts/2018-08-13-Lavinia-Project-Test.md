---
layout: post
title: Lavinia's summer project
subtitle: Is Steph Curry really in the 50 40 90 club?
gh-repo: SandyaS72/SandyaS72.github.io
gh-badge: [star, fork, follow]
tags: [test]
---

The [50-40-90 Club](https://en.wikipedia.org/wiki/50%E2%80%9340%E2%80%9390_club) is an elite distinction for basketball players who make 50% of field goal attempts, 40% of three point attempts, and 90% of free throw attempts over the course of an NBA season (with a minimum of 300 field goals, 82 three pointers, and 125 free throws made) intended to capture the best players of all time. As a representation of just how exclusive the club is, **50-40-90 seasons have only been accomplished eleven times** by seven different players over the course of nearly 40 years since the three point field goal was introduced. 

## The idea of uncertainty

There is always some chance involved in any single shot, game, or season. When a player goes to attempt a shot, there are many factors that contribute to whether or not the shot will be successful. Therefore, when a player takes a shot, it is not purely their ability that determines whether or not their shot will be successful. Instead, for each player there is a degree of uncertainty regarding their ability. We believe that the admission criteria to the club, as it currently stands, is not an accurate reflection of the pure skill level of a player, but rather also the “luck of the draw” of circumstances they happened to have faced that season. If a player makes 90.1% of their free throw attempts one season, how much of that can we attribute to their skill level as opposed to some combination of fortunate circumstances that gave them a few extra shots to make it past the threshold? If another player makes 89.9% of their free throw attempts, are they inherently less skilled? When taking a single sample, there is uncertainty and a single sample is subject to noise and random variation. 
  
What if you had to pick for your team between Player A who made 5 out of 10 (50%) field goals and Player B who made 50 out of 100 (50%) field goals? If we only consider their shooting percentages, we would say that both are equally good players and choose one randomly. But that doesn’t feel right, does it? 

The fact that they both have the same shooting percentage does not make them equally good players and this is why more than just shooting percentage has to be considered when answering this question. I would want Player B on my team because he has attempted more shots and still maintained the same shooting percentage. Therefore, there is less uncertainty regarding his shooting ability. Player B has attempted more shots and replicated successful shots more times, and because of that we feel more confidence in Player B’s ability to successfully throw free throws.  

For Player A, while not necessarily the case, it is much more likely that he had a series of lucky shots that happened to go in. Because 10 shots is such a small number of attempts, we don’t know if successfully making 5 out of 10 shots was pure luck, pure skill, or somewhere in between, whereas successfully making 50 out of 100 field is a lot more representative of actual shooting skill, rather than just luck. As the club currently stands, shooting percentage is the only factor that matters.

## A small thought experiment

Now, let’s say you called both Players A and B into a room and had them each attempt 100 field goals. What range would you be willing to put money on them being able to achieve?

Maybe you would be willing to bet on Player B making between 40 and 60 of his field goals, but would you be willing to say the same for Player A? Probably not. Based on your intuition alone, you picked a wider range for Player A than for Player B because there is more uncertainty about where Player A’s actual shooting percentage falls. If Player A had made just one more of his 10 shots, his shooting percentage would be 60%, and if he missed just one more shot, his shooting percentage would be 40%. One or two lucky shots could have significantly impacted his overall shooting percentage, which makes it difficult to pinpoint how well he can actually shoot. On the other hand, if Player B had made or missed one more shot, his shooting percentage would have been either 51% or 49% and only varied by 1%, as opposed to 10%. This is why when thinking about how many shots out of 100 Player A would make, there is less certainty. Through this, we arrive at the idea that more trials reduce uncertainty by examining the range within which you can be reasonably certain a player will shoot. 

## What determines uncertainty?

In the case of basketball scoring, what determines how certain (or uncertain) we are about a players scoring ability? When comparing Players A and B, we had less uncertainty about Player B’s scoring ability because he attempted more shots. For example, if Player B had made 5 out 100 shots, we would still be more certain about his scoring abilities than Player A’s, not because Player B made more shots, but because he attempted more. **Therefore, the uncertainty about a player’s scoring ability is based upon how many shots that player attempts, not the number of shots he makes.** 

{: .box-note}
**Key Takeaway:** Uncertainty depends on the total number of trials, not the number of successes.

## Margin of error

This is mathematically represented by the calculation for [margin of error](https://en.wikipedia.org/wiki/Margin_of_error) :
	\\[ ME=\frac{1}{\sqrt{n}} \\]
where n is the number of shots attempted.
	\\[ Player  A: ME=110=0.3162 \\]
	\\[ Player  B: ME=1100=0.1 \\]
What we arrived at earlier intuitively, we now demonstrate mathematically. For Player A, we can only be reasonably certain that his actual shooting percentage is within 0.3 of 0.5, but for Player B we can be reasonably certain that his actual shooting percentage is within 0.1 of 0.5.

## Confidence intervals

Because there is a degree of uncertainty that comes from taking just one sample, the margin of error says how much in either direction of the sample proportion our interval extends so that we can be 95% confident that, given the size of our one sample, the actual shooting percentage is in our interval. 95% confidence means that if we were to repeat random samples of the same size for our proportion of interest, 95% of them would capture the true proportion. 

If we were REALLY invested in figuring out the actual shooting percentages of Players A and B, we could take an infinite number of random samples of the same size. However, not only would this be extremely inconvenient, it would be outright impossible. Also, because the 50-40-90 Club is for shooting percentages over the course of one season, this option doesn’t make a whole lot of sense. Instead, we can use the sample proportion and sample size to do inference about the actual shooting percentages by constructing [confidence intervals](https://en.wikipedia.org/wiki/Confidence_interval) . A smaller margin of error is preferred because that means there is less uncertainty about where the true proportion falls.

{: .box-note}
**Key Takeaway:** With more attempts, it becomes less likely that players achieved a certain shooting percentage because of a few lucky (or unlucky) shots, and more likely that the player’s shooting percentage is representative of their skill.

## What does this mean for how we evaluate players? 

If a player just barely makes 50% of field goals or 90% of free throws, given the amount of uncertainty, we are not sure that they can actually shoot that well. We want to be 95% confident (read “reasonably certain”) that players can shoot at or above the threshold for inclusion in the club, to ensure that membership isn’t just granted based on a few lucky shots, but actual shooting ability. **However, for this to be true, players actually have to shoot above the threshold.**

But how much above the threshold to players have to shoot?

Given a confidence interval, the actual shooting percentage can fall ANYWHERE in the confidence interval. We can't be any more confident about values closer to the observed proportion than values further away within the interval. Therefore, **it is important that the entire confidence interval be above the threshold for inclusion in the club to ensure that a player can actually shoot as well as the club dictates.** Even if the lower bound of the confidence interval is 0.01 below the threshold for inclusion in the club, we cannot confidently rule out the possibility that the player's actual shooting percentage is in that small range below the threshold for inclusion in the club. 

So, how much better than the threshold will a player have to shoot to be admitted into the club? That will depend on the number of shots the player attempts. More shots attempted will lead to a narrower confidence interval, so the proportion observed won’t have to be as high for the lower bound of the confidence interval to be above the threshold for inclusion in the club. 

{: .box-note}
**Key Takeaway:** Players must actually shoot above the required thresholds for inclusion in the club in order to be 95% confident that their performance is actually above those thresholds.

## An Example

Looking at the confidence intervals for Players A and B below, we see that we can be reasonably certain that Player A makes above 19% of field goals and Player B makes above 40% of field goals, but, as discussed, this is not good enough to qualify for the 50% required by the club. 

![Player A](https://lh3.googleusercontent.com/JZi4BOAjDwbWkv5dP4VrBU5yszZK0CXyBXrtnx_3yintCOI8rDyuFUN733JSI31bXr3gMbQ9Mv1wgfaLUjv5nMCXKkMh4Q8iDWTKFT52GmJsRD3c0fI0GMfAnrH6hbtcyVmXrFh1=w2400)


![Player B](https://lh3.googleusercontent.com/0Jv_oPqwTic94Z7vGUbTggO5uk4GlHr5laI_zLynNOUI-OVp-d_PMOrUdVpnzzPaLvX1s_6L__G6E_FB72_c2jwiZPbSyu5TYIR7kpmWXnAKv0RVFCu6636-S_13lsBvORV5iWqI=w2400)

## The Bottom Line

To more accurately reflect the actual skill of the player, club membership should be defined in terms of the uncertainty (or lack thereof) around players’ performances in a season. This can be done using a confidence interval, which defines a range in which we are reasonably sure the player’s actual skill resides. Using confidence intervals inherently takes into account the number of shots attempted, since players who attempt fewer shots have to achieve a performance much higher than the cutoff to qualify, while players who attempt more shots decrease uncertainty and narrow that margin. Most importantly, this approach indicates our certainty in a player’s skill level, without just granting club membership based on a few lucky shots. 

When we take a look at the club this way, surprisingly, no player is qualified to be in the club. A few players currently in the club can qualify for one of the three types of shots, but no player can shoot at or above the cutoff for membership for all three types of shots with 95% confidence. 

{: .box-note}
**Key Takeaway:** No one makes the club.

**Table of All Players and Seasons claimed against Confidence Intervals**

| Player | Team | Season | FT % | FT confidence interval | FG % | FG confidence interval | 3P % | 3P confidence interval|
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |
