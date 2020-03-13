---
layout: post
title:      "Javascript Single Page Application"
date:       2020-03-13 09:50:47 -0400
permalink:  javascript_single_page_application
---


For my Javascript project I decided to make a memory card game with pictures of Bernie Sanders. As I mention with all my projects, this was a great project to really hone my javascript skills. The video provided to us was a video on how to make a note app that creates notes and displays notes. This was a great way to get my project started. That video only had 1 model to work with so everything was on same component and adapter. That was when I knew my project was gonna require a little out of the box thinking. My Bernie Game would require a User model and at least a Card model for the cards.

I started out with only the card model as I wanted to be able to provide seed data that would represent each card with unique face and then duplicate it. Each card has a front and back as well as a name (which will be used to check for a match). This was great way to start because I was able to use the similar code for displaying the notes from the video instead I used it to display the cards and fetch data from the rails api. 

As I began to develop the User model, I started realizing the structure of the Javascript files could possibly resemble the MVC structure of rails when using different models and adapters and components. For this model, I wanted to ask a User for their name so that I cuold create the user and then associate them with a game when user Starts Game (User has many games, game belongs to a user). My first major "bug" was when I would commit the User to the database, the SPA would refresh, which is the opposite of what we are trying to accomplish. After much time, I figured out it was because I was using a VS Code extension for Live Server that would refresh the page after every save or in this case commit. Once I created a new terminal and ran the server on HTTPserver I was able to finally get it to commit and not refresh the page. 

After these two models were creatad, I decided I wanted to make a game model that would be associated with the User and then when game was created, it would display the cards so that there is a clear order that must be followed. Another major problem I was having trouble solving was getting "this" to bind with the interval starter function that would determine a win or loss of game and update the game stats with proper information. After many google searches I found that a very simple fix is to simply create a variable (var _this = this) outside of the function and it can be called within it. This was the final logic that was needed in order to have a working game with scoreboard. 

Would love feedback from anyone interested in checking out my game. Please follow link below and clone! 

https://github.com/giancarloz/bernie-match


Best.
Giancarlo
