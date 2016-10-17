---
layout: post
title: Pomodoro Project
thumbnail-path: "img/pomodoroproject.png"
short-description: A time-management system based on the Pomodoro technique using AngularJS and Firebase

---

{:.center}
![]({{ site.baseurl }}/img/pomodoroproject.png)

## Explanation

The [Pomodoro Technique](http://pomodorotechnique.com/) aims to increase your work productivity and quality. In its simplest form, you time your work in 25-minute intervals, with five-minute breaks in between.

During a 25-minute session, you focus on a task. Checking email, answering the phone, or browsing your favorite forum is not allowed. During a break, you do not do anything related to work. You can meditate, do push ups and play with your dog, but you can't think about work.

When implemented with discipline, the Pomodoro Technique can be a powerful tool to increase your productivity.


## Problem

The first item to tackle in creating the Pomodoro time-management system, was to create the functionality desired by the timer. It would need to start the 25 minute work session, be able to pause, restart, and then automatically set to 5 minutes once complete. Similarly the 5 minute break session would need to be able to pause, restart, and then automatically set to 25 minutes once complete. Additionally, the application needed some way to create and persist tasks until complete.

## Solution

The application is built with an Angular framework and a UI-Router to connect the different modules, controllers, and services. The timer, with all of its functionality was organized as a service as was ultimately the task manager. To create and persist the tasks the application was connected to [Firebase](https://firebase.google.com/) using the given script snippet when the project was registered similar to the following:

{% highlight javascript %}
<script>
  // Initialize Firebase
  var config = {
    apiKey: "yourAPIkey",
    authDomain: "yourFirebaseDomain",
    databaseURL: "yourFirebaseURL",
    storageBucket: "yourFirebase.appspot.com",
    messagingSenderId: "yourSenderId"
  };
  firebase.initializeApp(config);
</script>
{% endhighlight %}

This connects to the Firebase API and allows the tasks to be created and destroyed via the web interface.

## Results

The application is able to consistently alternate between work sessions and break sessions with the ability to pause and restart a work or a break session. Additionally, having the application connected to Firebase allows the user to conveniently create a list of tasks and remove tasks as they become complete.

## Conclusion

The Pomodoro Project is a simple yet effective tool to help you focus and improve productivity. Firebase was a simple and effective solution to facilitate data persistence that enhanced the project overall.
