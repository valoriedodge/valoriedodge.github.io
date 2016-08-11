---
layout: post
title: My Second Alexa Skill
---

After [building my first Alexa skill]({% post_url 2016-07-27-building-an-alexa-trivia-skill.md %}), I was feeling pretty confident, and I was excited to build another one. This time I followed along the tutorial [How to Build a Fact-Based Alexa Skill](https://developer.amazon.com/public/community/post/Tx3DVGG0K0TPUGQ/New-Alexa-Skills-Kit-Template:-Step-by-Step-Guide-to-Build-a-Fact-Skill).

My first skill was a simple trivia game, built after the template Amazon outlined. The skill I built this time simply stated a fact from a given list when prompted. It really wasn't any more complicated than the first tutorial, and you can follow along without any prior experience with Alexa. It took me about the same amount of time, roughly a few hours. Again, most of my time was invested in choosing and creating a list of interesting facts for the skill to give when asked.

A major difference between deploying this skill and the last one, however, is that Amazon has created a [Software Development Kit (SDK)](https://developer.amazon.com/public/community/post/Tx213D2XQIYH864/Announcing-the-Alexa-Skills-Kit-for-Node-js). I was unfamiliar with SDK's and how they are useful. In a nutshell, alexa-sdk is a Node package that helps you build skills faster while allowing you to avoid unneeded complexity by handling things like session attributes, skill state persistence, response building and behavior modeling.

It wasn't too complicated to incorporate alexa-sdk. You just have to run `npm install --save alexa-sdk` within your Node.js environment. You can then import it into your app by including the following in your index.js file:
````
var Alexa = require('alexa-sdk');

exports.handler = function(event, context, callback){

    var alexa = Alexa.handler(event, context);

};
````
And if you are using Amazon's "space geek" template from the tutorial, they take care of that code for you.

By the end of the tutorial, I had built an amusing skill that states a crazy state law when prompted by the user. It's called Crazy State Laws (go figure, right?). Feel free to go and give it a try!
