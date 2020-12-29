---
date: 2020-12-29 14:30 +0100
author: locness3
title: "Getting started with Cloud Data : creating a global high score"
image: images/c-dustin-K-Iog-Bqf8E-unsplash.jpg
excerpt: "You want to show the highest score ever made in your game. Well, you just add a High Score variable, and if Score > High Score then set High Score to Score. That should work, right? Well, not really... Read on to find out more."
categories:
    - Tutorials
    - Tutorials/Cloud Data
tags:
    - cloud
    - cloud data
    - high score
    - ranking
    - scratcher rank
difficulty: Novice
---

So you made a great game, and you want to know who's the best at playing it.

Well, you will share it on Scratch, and you'll add a High Score variable, and if Score is more than High Score then set High Score to Score. This should work, right? If you test it you'll see it does. But... not really. It will not work with other people, except if you play in the offline editor or on the same account. 

Why? Because, when *you*, on your account or offline, change the variable's value, **Scratch will think you made a change to your project**, so it will save it. But other people aren't able to modify your project, so it won't save for them.

## This is where Cloud Data comes in!

Cloud Data lets you create **global, shared variables**, that everyone (with a Scratcher rank, see below) can modify, which you can use to save a global high score.

To be able to use Cloud Data, **you need to have a Scratcher rank on the Scratch website.** This applies to you and to those who play your project : they can't change these variables without the Scratcher rank.

<!-- To be wrapped in a callout -->
Cloud Data variables can only be numbers, and cloud lists aren't a thing, but there are workarounds which I won't cover here yet.

To have this Scratcher rank, you have to be active in the Scratch community, have a verified email address, and at least 2 shared projects. More on that [here](https://en.scratch-wiki.info/wiki/New_Scratcher_Status#Requirements_for_becoming_a_Scratcher).

Now, let's get started and create a simple highscore system!

## Creating a cloud variable

First, open your project. Go to Variables and click `Make a Variable`. Name the variable `High Score`. **Be sure to check `Cloud variable (stored on server)`**, otherwise it will not be a cloud variable.

You will see the variable alongside other variables, and its name will be preceded with a ☁︎ symbol. This means it's a cloud variable.

Now, at the end of the game, do a check to verify if the score is superior to the high score, and if yes, update the `High Score` variable, just like you would do as usual.

As you can see, Cloud Data is really easy to get started with.