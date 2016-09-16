---
layout: post
title: Building Baby Logs
---

Another Alexa skill? Yep! I told you I'm in love. It is so fun to be able to build something that is useful and practical and that is why I created Baby Logs. I decided to build Baby Logs as a natural successor to Pregnancy Countdown. It is an app for after the baby arrives.

As a mom, it is so hard to keep track of when I put my baby or toddler down for their nap, or how long they slept. Also, I always have a hard time keeping track of how long ago I nursed or fed my child. And when they were newborns or sick and the nurse asked me how many dirty diapers in the past 24 hours they had had I could never remember. All of these problems are the inspiration behind Baby Logs. Baby Logs is an app that will keep track of when a baby eats, sleeps and has a dirty diaper.

Most of the challenges I faced in creating Baby Logs were similar to the ones I overcame in creating Pregnancy Countdown. I still needed to persist data for each user. I also needed to create methods to retrieve and process data to give valuable output. I wanted to be able to tell a user when a child went down for a nap, when they woke up, when they last ate, or how many dirty diapers they had. These are things that all parents have a hard time keeping track of, especially sleep-deprived parents of newborns.

A unique problem I had to solve with Baby Logs was figuring out how to save a lot more data than just a due date in DynamoDB. I had to figure out how to organize the data to make it the most accessible. I decided to create an array of children's names so potentially a user could keep track of activities for more than one child. Then I created objects for the naps, feedings, and diapers. The key in the object was the child's name and the value was an array of saved events.

I have to say, it is another pretty basic skill, but useful for parents of young children everywhere. Actually, it can really track the feedings and sleeping and dirty diapers of anyone, so feel free to try it out!
