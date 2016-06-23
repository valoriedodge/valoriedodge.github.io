---
layout: post
title: Blocipedia
thumbnail-path: "img/blocipedia.png"
short-description: Build a production quality SaaS app that allows users to create their own wikis.

---

{:.center}
![]({{ site.baseurl }}/img/blocipedia.png)

## Explanation

People are always looking for new ways to collaborate in order to create products and resources that can also be shared with others. Blocipedia was created as a resource to facilitate the sharing of knowledge and skills to build both public and private wikis, which also allow markdown syntax. These wikis can be kept private with collaborators added as needed, or they can be made public allowing anyone to give input and improve the content of the wiki.


## Problem

Building the application from scratch, I had to initiate the application and create all of the necessary models and controllers. Multiple users can be assigned to the same wiki but in a number of different capacities. I needed the ability to identify users as the creator, contributors, and assigned collaborators. Additionally, I needed a way to process payments to upgrade users to premium. Only premium users are allowed to create private wikis, creating the need to discriminate between users, as well as identify which wikis are public and which are private.

{:.center}
![]({{ site.baseurl }}/img/Wiki Homepage.png)

## Solution

Before beginning, I organized my application with its databases to store the information I needed to build a functioning site. I created a collaborations join table and then built my relationships between users and wikis through that table.  I employed the Ruby gem pundit and then built filters to help create scopes for allowing certain users to be able to access and contribute to specific wikis. I also used stripe.com to process payments for user upgrade. Afterward, I had to ensure that if a user chose to downgrade, any of their private wikis were made accessible.

## Results

All of the functionality of the website was developed using Test Driven Development. I wrote encompassing tests for all of the functionality of the application to ensure that it was behaving as I intended. The application was also tested locally before it was put into production on Heroku and tested for functionality there as well. Users were successfully able to create and contribute to wikis after signing up for an account. They were also able to upgrade their account to premium and create private wikis where they could add other users as collaborators.

{:.center}
![]({{ site.baseurl }}/img/Wiki Tests.png)

## Conclusion

Though basic in functionality, Blocipedia satisfied the scope of creating a tool where users could create and collaborate on public and private wikis. Stripe was an excellent resource, making processing payments a breeze. Moving forward, the design and layout of the application has plenty of potential for improvements.
