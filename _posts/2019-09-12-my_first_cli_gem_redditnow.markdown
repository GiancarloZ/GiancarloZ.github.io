---
layout: post
title:      "My first CLI GEM: RedditNow."
date:       2019-09-12 18:53:00 +0000
permalink:  my_first_cli_gem_redditnow
---


Hello World, 

I just created a CLI Data Gem for my Ruby final project. 

I always knew which website I was going to scrape as I'm on it far too often and that of course is Reddit.com. At first, I had no idea how I'd begin creating this program as this is the first lab/project where you have to build something from scratch. Luckily, this course provides great videos and the lessons leading up to this project have really been ingrained in my brain. Once I actually began (I have to admit took me a day or two to actually commit to starting this project) it started to flow.

I started off with the CLI code as I had an idea of how I wanted it to look and run. I created a basic menu and a fake "post" text so that I could just get the program working and looking how I wanted before actually creating the post.rb file to actually scrape the data and bring it in. Now, the hard part truly was the scraping. On the previous scraping lessons and videos, Avi always mentions how every website is different and how it can really be a pain sometimes to scrape. I didn't quite understand what he meant by that becuase the sites we were scraping didn't seem to complicated. Oh how right he was. Reddit's code was a nightmare at first to understand and grab exacly what I wanted. There was not basic single class or ID word that was unique amongst every post. I saw div code in there that I have never seen before. But with enough time and a lot of binding.pry testing I managed to get a grasp and once I did it was actually quite easy to find and grab what I needed! It really is projects like these that truly teach you things you thought you knew but really didn't. 


In Reddit_now, you can run ./bin/setup to install all gems and run program with ./bin/reddit-now. When you run the program it will populate the top 25 reddit posts on r/all at that moment. It will list out each post with the amount of upvotes it has, the title, which subreddit it was submitted and by which user. Choose the post you'd like to see by typing in the post number and go to the link it provides. I hope you all enjoy. 

Feel free to check it out and any feedback in preferred! 
Link: https://github.com/LadanZiaee/reddit_now

Best,
Giancarlo
