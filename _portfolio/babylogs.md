---
layout: post
title: Baby Logs
thumbnail-path: "img/BabyLogs.png"
short-description: An Amazon Alexa Skill to help new parents track baby activities built with ASK and Node.js

---

{:.center}
![]({{ site.baseurl }}/img/BabyLogs.png)

Icon made by Roundicons from www.flaticon.com

## Explanation

New parents often find themselves asking how long their baby has been sleeping, or when their last nap was, or maybe when they ate last or how long they nursed. In the first few weeks or whenever the baby becomes ill, the nurse or doctor will probably inquire how many dirty diapers the baby has had in the past 24 hours. Baby Logs is an [Amazon Alexa](https://www.amazon.com/Amazon-Echo-Bluetooth-Speaker-with-WiFi-Alexa/dp/B00X4WHP5E) skill built to help all parents track each of these events. Baby logs will track when and how long a baby eats or sleeps, as well as track and report the number of dirty diapers recorded in the past 24 hours.  


## Problem

The main challenge in building this Alexa skill was being able to structure and persist the user's data for the individual events. The skill needed to be able to save and retrieve information on command. This proved complicated when evaluating the time passed since the saved event and returning it in a comprehensible format.

## Solution

Baby Logs uses the Alexa Skills Kit basic object and then connects to DynamoDB to persist user data. The DynamoDB table is structured based on the individual User ID, assigned by Amazon, and then contains a name array for users to register the children they would like to track along with individual objects for eatings, feedings, and diapers.

## Results

Baby Logs is an active Amazon Alexa Skill able to effectively record and report the feedings, naps, and dirty diapers of any number of children.

## Conclusion

Baby Logs is a unique and useful solution to help simplify the lives of parents by tracking common baby activities and providing the information upon request.
