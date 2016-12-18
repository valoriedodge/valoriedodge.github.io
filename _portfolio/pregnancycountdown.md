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

Excited expectant parents are continuously asking themselves how much longer until the baby arrives or wondering how big their little sprout is. Pregnancy Countdown is an [Amazon Alexa](https://www.amazon.com/Amazon-Echo-Bluetooth-Speaker-with-WiFi-Alexa/dp/B00X4WHP5E) skill built to help these anxious parents know the answers to those questions simply by asking. Pregnancy Countdown will record the baby's due date and then give the size of the baby or the time left in the pregnancy upon request.


## Problem

The main challenges in building this Alexa skill was learning how to structure the code using Node.js and Amazon's Alexa Skills Kit as well as being able to persist the user's data for the due date. The skill needed to be able to save and retrieve the due date as well as process specific requests as given by the user.

## Solution

Because I had already chosen to use the AWS Lambda function to house Pregnancy Countdown, I decided to also use Amazon's DynamoDB to persist user data. Pregnancy Countdown uses the Alexa Skills Kit basic functionality and then connects to DynamoDB to save the user's due date. The DynamoDB table is structured based on the individual User ID assigned by Amazon and then contains a name array for users to register the baby's due date. From there, I patterned my code after Amazon's sample codes to create the desired functionality of offering the size of the baby and the time left when asked by the user.

## Results

Pregnancy Countdown is an active Amazon Alexa Skill able to effectively record a user's due date as well as provide how far along the pregnancy is, how much time remains, and the approximate size of the baby in weight, height, and fruit size.

## Conclusion

Pregnancy Countdown is a unique and useful solution to help simplify the lives of expectant parents by providing simple information based on the given due date. DynamoDB was a simple and very effective solution to incorporate in the Alexa skill to allow the persistence of user data.
