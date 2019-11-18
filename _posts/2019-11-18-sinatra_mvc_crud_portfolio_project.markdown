---
layout: post
title:      "Sinatra MVC CRUD Portfolio Project"
date:       2019-11-18 14:46:16 +0000
permalink:  sinatra_mvc_crud_portfolio_project
---


My first real web application! It was easy coming up with an idea for this project as all my immediate family members are/were in someway a doctor. My brother is in reidency  for Psychiatry and I figured I'd make him a web application that he could sign into to view and prescribe medications for his patients and his patients could log in to view who their doctor was and what medications they prescribe (and maybe later make it so they could video chat for a session or send the medication to their pharmacy...but not lets get ahead of ourselves). 

I knew this Idea would meet all of the requirements but I did not realize how much different and more advanced it would be than the Fwitter/PLaylister labs we had done prior. It was only when I sat down to write out how I would make the associations and build the actual website did I realize that I would need to tweak and add a lot more features from those previous labs than originally intended which is why it took just a little bit longer to complete but I'm very happy for having completed it. 

The has_many and belongs_to properties were quite similar to the Playlister Artist/song/genre models so that came rather easy. The parts where I felt required a little more problem solving were when I got to log in pages and show/edit pages. I know that I needed a different login area for Doctors and Patients as I realized Patients shouldn't be able to edit what medications they were prescribed as that could lead to some abuse. So I needed to add a logged_in? helper method but also include whether or not the session[:id] and session[:username] could be found in Doctor table or Patient table to block a certain user from viewing certain pages depending on who was logged in. I needed to have slightly different paths in my controllers becuase a Patient user would only be able to edit/delete their account (such as an account settings feature) so would only need to have /patients/:id path as we've been taught. But for a doctor, they would need to slug their username so if they were to click on a patient, it would need to lead to  "/doctors/:slug/:id" where slug is their username and id was the pateints ID. The doctor could also edit/delete his own account. 

The best part of the two projects I've done is that they end up teaching you and making you feel so much more comfortable with certain features or codes that it really engrains them into your mind. The CLI Project actually taught me how to really use binding.pry (i'll admit that every time a lesson or a video lesson mentioned using it or showed you how they used it, my mind would just skip over it as I had no idea how or what to do with it). After trying to scrape a webpage for certain features I need a more efficient way of understanding what my variables were grabbing. This Project has taught me exactly how controllers work, how to use flash messages, how to grab and manipulate join tables, and using migrations to change column names or data type. I'm very happy and excited about completing this project all on my own and would love some feedback from other Flatiron School coders. Feel free to clone the repo below and test it out! 

git@github.com:GiancarloZ/med-app.git

Best,
Giancarlo
