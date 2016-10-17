---
layout: post
title: Pregnancy Countdown
thumbnail-path: "img/PregnancyCountdown.png"
short-description: An Amazon Alexa skill to help expecting parents built with ASK and Node.js

---

{:.center}
![]({{ site.baseurl }}/img/PregnancyCountdown.png)

{:.center}
Icon made by Roundicons from www.flaticon.com

## Explanation

Excited expectant parents are continuously asking themselves how much longer until the baby arrives or wondering how big is their little sprout. Pregnancy Countdown is an [Amazon Alexa](https://www.amazon.com/Amazon-Echo-Bluetooth-Speaker-with-WiFi-Alexa/dp/B00X4WHP5E) skill built to help these anxious parents know the answers to those questions simply by asking. Pregnancy Countdown will record the baby's due date and then give the size of the baby or the time left in the pregnancy upon request.


## Problem

The main challenges in building this Alexa skill was learning how to structure the code using Node.js and Amazon's Alexa Skills Kit as well as being able to persist the user's data for the due date. The skill needed to be able to save and retrieve the due date as well as process specific requests.

## Solution

Baby Logs uses the Alexa Skills Kit basic functionality and then connects to DynamoDB to persist user data. The DynamoDB table is structured based on the individual User ID assigned by Amazon and then contains a name array for users to register the children they would like to track along with individual objects for eatings, feedings, and diapers.

## Results

Baby Logs is an active Amazon Alexa Skill able to effectively record and report the feedings, naps, and dirty diapers of any number of children.

## Conclusion

Baby Logs is a unique and useful solution to help simplify the lives of parents by tracking common baby activities and providing the information upon request.
