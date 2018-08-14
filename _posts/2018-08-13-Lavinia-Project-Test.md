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

  There is always some chance involved in any single shot, game, or season. When a player goes to attempt a shot, there are many factors that contribute to whether or not the shot will be successful. Therefore, when a player takes a shot, it is not purely their ability that determines whether or not their shot will be successful. Instead, for each player there is a degree of uncertainty regarding their ability. The admission criteria to the club, as it currently stands, is not an accurate reflection of the pure skill level of a player, but rather also the “luck of the draw” of circumstances they happened to have faced that season. 

  If a player makes 90.1% of their free throw attempts one season, how much of that can we attribute to their skill level as opposed to some combination of fortunate circumstances that gave them a few extra shots to make it past the threshold? If another player makes 89.9% of their free throw attempts, are they inherently less skilled? When taking a single sample, there is uncertainty and a single sample is subject to noise and random variation. 

  What if you had to pick for your team between Player A who made 9 out of 10 free throws and Player B who made 90 out of 100 free throws? If we only consider their shooting percentages, we would say that both are equally good players and choose one randomly. But that doesn’t feel right, does it? The fact that they both have the same shooting percentage does not make them equally good players and this is why more than just shooting percentage has to be considered when answering this question. 

  I would want Player B on my team because he has attempted more shots and still maintained the same shooting percentage. Therefore, there is less uncertainty regarding his shooting ability. Player B has attempted more shots and replicated successful shots more times, and because of that we feel more confidence in Player B’s ability to successfully throw free throws. For Player A, while not necessarily the case, it is much more likely that he had a series of lucky shots that happened to go in. Because 10 shots is such a small number of attempts, we don’t know if successfully making 9 out of 10 shots was pure luck, pure skill, or somewhere in between, whereas successfully making 90 out of 100 free throws is a lot more representative of actual shooting skill, rather than just luck. Of course it is possible that Player B just had a series of lucky shots, but given he attempted 100 shots, this is a lot less likely. As the club currently stands, shooting percentage is the only factor that matters.


Here is an example of one player's score 

![PlayerA](https://drive.google.com/file/d/16ANYMJOTkBxbiO8_RkfiPHK7-lxo913W/view?usp=sharing)

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
