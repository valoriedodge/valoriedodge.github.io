---
layout: post
title: Flash Photographer
thumbnail-path: "img/FP Home.png"
short-description: An application that allows users to search for photographers based on zip code.

---

{:.center}
![]({{ site.baseurl }}/img/FP Home.png)

## Explanation

It can often be difficult to find a photographer, especially when it is for an event outside your immediate location. People spend too much time and money searching different sites and using other resources to find a photographer that will fit their needs. Often people will pay huge travel expenses for photographers because information on photographers in the location they are seeking is unreliable. Creating a centralized location for photographers to create profiles and list their information not only will help them increase their clientele, but will help users save time and money by giving them one site to find and compare photographers to find the one that is just right for them. Including user reviews gives reliability to the site and helps ensure the quality of the photographer for the users.

{:.center}
![]({{ site.baseurl }}/img/FP Home 2.png)

## Problem

Building the application from the ground up, I had to initiate the application and create all of the necessary models and controllers. I also had to create the design and layout. I needed two types of users to be able to create accounts and subsequently login. Photographers needed to be able to create profiles with all of their information. Users needed to be able to search photographers by location. Finally, users needed to be able to leave reviews for the benefit of all involved.

## Solution

I decided to create two user models for the application through the Ruby gem devise. Because the information I needed from the two types of users was quite different and I needed them to be able to interact independently, that it made it prudent to actually create photographers and users as two separate user models. Initially, I created a search model that would record user searches by zip code; however, I changed it to simply pass the zip code as a parameter to filter the list of photographers indexed. I also created a review model where users can designate a 1-5 rating and leave a review for any photographer.

{:.center}
![]({{ site.baseurl }}/img/Photographer Login.png)

{:.center}
![]({{ site.baseurl }}/img/FP Search.png)

## Results

All of the functionality of the website was developed using Test Driven Development. I wrote encompassing tests for all of the functionality of the application to ensure that it was behaving as I intended. I included simplecov to track the coverage of my tests and overall it was covered above 98%. The application was also tested locally before it was put into production on Heroku and tested for functionality there as well. Photographers are able to create profiles and users are able to search for photographers based on zip codes. Users are also able to successfully leave reviews.


## Conclusion

Having two user models was very effective for the scope of the site. Searching by zip code was effective, though it would be much nicer to also be able to search by city and state. Creating the 1-5 rating was much more difficult than expected, after trying several solutions, I finally accepted the given rating solution. Going forward, it would also be nice for photographers to expand their profile to include examples of their work, their price points for different events, and even a calendar with their availability. Also, there is always room for improvement on the design, particularly for the images to display appropriately regardless of screen size.
