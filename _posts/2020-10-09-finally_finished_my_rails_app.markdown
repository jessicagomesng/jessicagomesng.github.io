---
layout: post
title:      "Finally Finished my Rails App!"
date:       2020-10-09 14:16:06 +0000
permalink:  finally_finished_my_rails_app
---


My gosh! I am so pleased to be writing this blog post and to be *officially* finished with my Rails app! This took me so much longer than anticipated, but I think I'm pretty happy with what I've created! 

I had a difficult time coming up with an idea for my application at first. Initially, I wanted to create a registry application where users could create wishlists and add items to their wishlists. This started to get complicated when I realised users could either take on the role of buyer or seller. I couldn't figure out how to represent this relationship, and it just kept getting more and more complicated!

I started to lose interest in that idea the more I tried to make it work, so I turned back to the drawing board! In the end, I came up with the idea to create an event booking application. My usual work is in theatre, so it seemed like something that aligned closely with principles I already understood. Even though all events will probably be on hold for a little while, I thought this idea was pretty functional. I again had problems because I wanted the app to have both users and producers, but I couldn't decide if they should all be housed under one model class with the admin option. In the end, I decided to keep them separate because I had different belongs_to and has_many relationships for each one!

I learned a lot throughout this process. One of the biggest challenges I faced was adding the Omniauth login -- I wanted to extract a Facebook user's birthday and email information in order to create their accounts, and I initially kept running into dead ends! Several hours (and many highly useful *Medium* articles) later, I finally figured out how to do this, and I am pretty pleased overall with the result. 

The other biggest challenge I faced was figuring out how to DRY my code. I felt like there were a lot of places where code could have been condensed, and I also sometimes couldn't quite figure out how to best apply separation of concerns to my application. I'm still not totally sure that I nailed this, and I'm sure my project review will illuminate many places in my code that can be refactored to be more concise or rearranged. 

Overall, I'm very glad to be done and moving on to something new!
