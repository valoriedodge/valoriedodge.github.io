---
layout: post
title: BlocJams
thumbnail-path: "img/blocjams.png"
short-description: A digital music player built with Angular.js

---

{:.center}
![]({{ site.baseurl }}/img/blocjams.png)

## Explanation

BlocJams is a digital music player like [Spotify](https://www.spotify.com/us/), created as a means to learn frontend web development. It employs a user-friendly web interface to display and play songs. The mp3 files are accessed through BuzzFeed sounds and the application is built within an Angular framework.

## Problem

The main task was to learn how to incorporate and build the entire application using the Angular framework. It was challenging to learn how to initiate Angular modules, controllers and services. It was also difficult to learn and appropriately apply the different types of services. Finally, I had to learn the Angular directives to use in the html pages in order to have the desired functionality.

{:.center}
![]({{ site.baseurl }}/img/blocjamsalbum.png)

## Solution

The site was centered around one Angular module built with a UI-router to connect the different controllers and services. The controllers were organized according to the different pages within the application- one for the landing page, one for the collection of albums, and one for the album page that lists the album songs. A player-bar controller was also created to compartmentalize the functionality of the bottom bar and incorporate it in the appropriate views.

## Results

The application is fully functioning with the ability to navigate between the different pages. The song player will play songs upon request with the ability to stop, pause, skip to the next/previous song, skip to a later point in the song, and to control the volume.

## Conclusion

Angular was an efficient way to build this web based music player. BuzzFeed sounds made simple music tasks such as start, stop, and play easy. The UI-Router was an easy and efficient way to structure the application that made the single page application very effective.
