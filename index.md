---
title: Manoa Bazaar
---

## Table of contents
* [Overview](#overview)
* [Goals](#goals)
* [Features](#features)
* Current App Pages:
  * [Landing Page](#landing-page)
  * [Categories Pages](#categories-page)
  * [User Profile Page](#user-profile-page)
  * [List Item page](#list-item-page)
  * [Admin](#admin)
* [Developer Guide](#developer-guide)
* [Community Feedback](#community-feedback)
* [Team Members](#team-members)

## Overview
The Manoa Bazaar is an application for UHM students to facilitate buying and selling of student-related goods and services. Check out our [Organization Page](https://github.com/manoa-bazaar) as well as our [Milestone 1](https://github.com/manoa-bazaar/manoa-bazaar/projects/1), [Milestone 2](https://github.com/manoa-bazaar/manoa-bazaar/projects/3), and [Milestone 3](https://github.com/manoa-bazaar/manoa-bazaar/projects/4) pages to follow along with our progress! You can see a development version of our website [here](https://manoabazaar.com/). Our TestCafe badge is ![ci-badge](https://github.com/manoa-bazaar/manoa-bazaar/workflows/manoa-bazaar/badge.svg).

## Goals
A big problem many students face is the high turnover rate of goods purchased throughout their semesters at UH Manoa. Our goal is to create an interface to help students buy and sell products easily, without having to worry about the usual problems that come with using mainstream reselling companies such as high shipping costs and long shipping times.

## Features
The Manoa Bazaar application will allow users to upload images of the items that they are selling, and each user will have a profile page which lists all of the items that they are selling as well as their rating.

### Landing page  
The [landing page](https://manoabazaar.com/) is presented to users when they visit the top-level URL to the site.
It displays a list of most highly viewed items that are currently being sold at the top level, followed by categories that display related items.

![Landing](mockup-pictures/Landing.JPG)

As you can see in the top right of the landing page, there is the option to login or to register. When you click on login, you can login using your credentials. If you don't have am account yet, you can click on sign up. 
The login page looks like this:

![Login page](mockup-pictures/signin.JPG)

The register page looks like this:
![Register page](mockup-pictures/signup.JPG)


### Categories page 
Once the user is logged in, they can see the different categories in which items are offered.
The [Categories page](https://manoabazaar.com/#/categories) shows ths users 5 categories: textbooks, kitchenware, bedroom items, school supplies, and other items. The first 4 categories contain items that fall into each of the categories, and the "other items" category holds items that don't belong in any of the other categories. Clicking on each of these categories takes you to a page of that category, where the items are listed. 

![Category Examples](mockup-pictures/categories1.JPG)

When you click on the category you are looking for, it will take you to a page where the items for that category are listed. When you click on the [Textbooks](https://manoabazaar.com/#/textbooks) category, the page will display the textbooks currently being offered. Each item has a button at the bottom that says "view item", that when clicked on, will take show you the item with all the details belonging to that item. This is the same for all items in each of the categories. In the case of the Textbooks category looks like this:

![Textbooks Category View item](mockup-pictures/rtextbooks.JPG)

It shows all the textbooks that are offered on the Manoa-Bazaar app. 
Each of the categories, when clicked on, will have their own page that displays the items that are listed in that category, and each item on that page has a button that links to the view item page.

### User Profile page  
The user profile is shown when you click on a user's picture or name. It displays their banner picture, icon picture, username, average rating, amount of items currently being listed and total sales, and a short description of their shop. The rating can be clicked to see reviews left by other users. Here is a link to that page: [https://manoabazaar.com/#/user-profile](https://manoabazaar.com/#/user-profile)

![User Profile](mockup-pictures/user-profile-mock-1.png)

A better picture of the items currently being listed.
![User Profile](mockup-pictures/user-profile-mock-2.png)
I plan on implementing a separate tab that shows the list of already sold items.

### List Item page 
Page that allows users to list their own items for sale, this item is to be displayed on their profiles and respective categories. 
Gives users options to choose caregories, prices, and input descriptions. 
(available [here](https://manoabazaar.com/#/add))

The add listing page looks like this:

![Creating an Example Listing](mockup-pictures/listitem.JPG)

When the information is filled out, you click submit. An alert will appear on the screen that the item has been added successfully. 

![Listing-added](mockup-pictures/listitem1.JPG)
![Alert listing](mockup-pictures/listitem2.JPG)

Then, the listing appears in the page of the category it was added in:

![Page of listing](mockup-pictures/ntextbooks.JPG)

### Admin
When the current user logged in has the role admin, there are some extra things the admin can do. The admin has an extra tab in the menu that says "[Admin](https://manoabazaar.com/#/admin)". When the user clicks on that page, all the listings will be displayed on that site, including the option to edit or delete that listing. The admin can also see who the owner of that listing is:

![Edit listing](mockup-pictures/admin1.JPG)

The admin can edit and remove listings. When the new information is put into that page, you click 'submit', and then you'll get a notification that the item has updated successfully (in this case, we've updated the price):

![Alert edit](mockup-pictures/editlisting2.JPG)

Now, as you can see, the price of the first listing has been updated:

![Updated listing](mockup-pictures/editlisting3.JPG)

The admin also has the power to remove items. The item we added in Add Listing page, the French textbook, appears in the Admin tab:
![Listing in admin page](mockup-pictures/listing-in-admin.png)

Then, when you click on remove, it is removed:
![Listing removed](mockup-pictures/listing-removed.png)

### Developer Guide
First, install [Meteor](https://www.meteor.com/install).

Second, visit the [Manoa Bazaar application github page](https://github.com/manoa-bazaar/manoa-bazaar), and click the “Code” button that gives you the option to clone the code to your computer.

Third, clone the code onto your computer and name the repository.

Fourth, cd into the app/ directory of your local copy of the repoand install the required libraries using

```
$meteor npm install
```
Lastly, run the system with:

```
$meteor npm run start
```
Your application will appear at [http://localhost:3000](http://localhost:3000).

### Initialization
There will be a default set of data that will be created the first time the app runs. 
If you add your own item listings it should appear in the terminal after you reset the application using.
```
$meteor reset
```

### Development History 
Milestone 1: [Click Here](https://github.com/manoa-bazaar/manoa-bazaar/projects/1)

The goal for Milestone 1 was to complete the development of various pages such as the landing page, user profile page, etc. The website was also deployed with a unique url.

Milestone 2: [Click Here](https://github.com/manoa-bazaar/manoa-bazaar/projects/3)

The goal of Milestone 2 is to improve the website's functionality by adding additional pages and implementing realistic datasets. 

Milestone 3: [Click here](https://github.com/manoa-bazaar/manoa-bazaar/projects/4)

The goal of Milestone 3 is to have a functional website that satisfies the goals of our project. 

## Community Feedback 
Manoa bazaar is a website that is made by us for our community members. We've asked some community members what their opinion about Manoa Bazaar is. Here is what they had to say. 

> I really like the idea of Manoa Bazaar. It is super convenient so have all items in one place, instead of all over facebook / going around in text groups.
Manoa Bazaar is an userfriendly site. It was pretty easy for me to navigate on the website, and I like how the items are divided up into categories. Maybe a nice feature would have been if the categories were divided up into further subcategories. For example, when you are looking for a textbook, you have to look through the whole page of the textbooks to find books for a certain subject.

-- Anne, Communications major 

> This is such a good idea for a website! I've been using facebook marketplace to try and sell items when I moved out of the dorms, but it didn't work that well. This is an organized website that displays the items that are currently being offered. Adding a listing is very easy, and it is nice that the item immediately appears in its respective category. That way, people can see your item very soon and it will probably sell faster.

-- Carmen, Sociology major 

> I really like that this is a website by UHM students for UHM students (and faculty). That way, you know that all the items you see are close by. There are no super long shipping costs, and it would even be possible to have an item the next day. This just all seems very effective, and I like that the products stay within the community. 
The website is easy to navigate and understand. I like that the landing page displays some items, so you can get a feel for what is offered on the website. I'm not sure if these items have any meaning, such as most viewed or most popular items, and if not, I think that would be a cool thing to add. I think that would give users a better insight into the website and what items would do well on there.

-- Irene, KRS major

> It is a cool idea and development. There are some cosmetic things, in my opinion, that could improve the look and feel of the website. For example, on the view item page, the button to view the item is a different height on each seperate item. If this were to be the same on all the items, I think it would give the website a more professional feel.
Besides those little appearance things, the website works well. It's awesome that it offers items from UH students for UH students. The items are displayed in an organized way, and I like that you see more details when you click on the item and that you can make a bid there! I like the bidding concept, because it can increase the value of an item if it is really popular.

-- Josh, Mathematics major

> The website is easy to use. I like how simple adding and editing a listing are. I like how you can bid on an item, it seems similar to facebook marketplace where UH students also sell and buy items, but here all the items are in one place. I like how there are five categories and each of these categories are very broad and simplistic. However, when furniture is offered, I don't know if I should put it in bedroom items, or other items. Maybe there could have been another category for furniture. 
I would also recommend changing the view item button on each of the items to stick to the bottom of the item. 

-- Mary, Mechanical Engineering major

## Team Members
<img src="https://avatars2.githubusercontent.com/u/70424200?s=460&u=78fa4d13c46fa5000026c3dc1d8147890934ff8b&v=4" width="200">

Daniel Kim:
This project seems like an excellent time to practice time management as well as splitting larger problems down into smaller ones. I hope to gain better insights into the software development process as well as improve my communication skills with my teammates. 

<img src="https://avatars3.githubusercontent.com/u/70546449?s=460&u=3ed8f860ad375ed8023b0788feb719d76230a787&v=4" width="200">

Emma van Rossum: 
I am really excited to better my software engineering skills during this project and to work with my peers to create a cool app that has good functionality. I hope to, like Daniel, gain a better understanding of the software engineering process. What I've seen so far of the process in this class, I really liked and thought was really interesting. I think this project is a great first project and I am excited to see what I'll learn from this. 

<img src="https://avatars1.githubusercontent.com/u/59942681?s=400&u=5385a63576924fa39d204fa624b6a152e9201ad5&v=4" width="200">

Lana Kawauchi:
I am currently majoring in ICS . I am looking forward to creating a fully functional website with the help of my project members. Before the pandemic I would often visit swap meets and farmers markets so I am excited to see how we can develop our website into something that can possibly help students in the future. 

<img src="https://avatars1.githubusercontent.com/u/34012125?s=400&u=8591666b03cf1017302a1898dd88ee57817aa37a&v=4" width="200">

Lian Huang:
I am excited about working with my teammates to build a fully functional website from the concepts we learned in class. This project presents a great opportunity to get a feel for what role I’d do well in and enjoy in a team environment. 


