---
layout: post
title:      "Sinatra Web App Project"
date:       2020-06-28 12:40:35 +0000
permalink:  sinatra_web_app_project
---


Wow!! I am really behind on writing this blog post and also on submitting my web app. I've been sick for the past two weeks, so I've just been slogging through and trying to get everything finished. 

This web app was a lot of fun to make! I feel like I've learned a lot since the very first project -- I think I'm starting to understand directories a lot more and necessary files in applications, which makes these projects a lot easier. I do wish these things were explained in a bit more detail, since a lot of stuff just required a lot of googling to understand. 

I ended up starting this project by looking at previous labs and basically copying the file structure there that was already present. Whenever I watch the lectures or video reviews, I'm always impressed by how Avi already knows all of the files that should be present and what to put in them. He always prefaces things by saying he's been coding for a long time, but it kind of makes me think I should have a better understanding of what goes where and exactly why it's there. Again, I think that there are some holes in terms of explanation in the course. Some of the documentation out there is verbose and kind of difficult to understand when it comes to explaining file structure, so I feel like it would be helpful to have more in the curriculum on this and more practice on it in general! 

One of my biggest challenges in writing my application was figuring out how to automatically add in some instances of the Symptom class that would populate my app. I initially had a whole other class that created Symptoms when the app first started, but that caused a lot of problems in my migrations, so I ended up just adding the instances into the seed file and instructing the user to also run *rake db:seed* after running the migrations. Hopefully, I'll learn about different solutions for this in my project review. 

I also ran into some problems trying to get my stylesheet to work in my application. I ended up starting out by using an internal stylesheet in my layout.erb file and then eventually figuring out how to link to it. I think the biggest issue is that I was trying to link to "index.css" instead of "/index.css". I read something about how the latter is an absolute path whereas the first is a relative path, and it wouldn't work in the former case but would in the second. Anyway, after trying out about a thousand iterations of this link path, I ended up getting it to work out, so we're good on this front too! 

Anyway, I don't really have much else to say about making this application -- I'm excited to move on and learn more now! 
