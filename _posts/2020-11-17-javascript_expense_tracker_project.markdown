---
layout: post
title:      "Javascript Expense Tracker Project"
date:       2020-11-17 16:54:33 +0000
permalink:  javascript_expense_tracker_project
---


I've just submitted and completed the JS Expense Tracker Project! These projects always take me so long to do -- I always have lofty goals of finishing them early, but I think I end up really obsessing over details and so stretching out the length of time before the project is officially 'completed'. Also, the more complicated these applications get, the more I feel like I'm missing something upon submission -- did I test every route via every possible iteration? 

The reason this project took me so long is also that I wanted to clean up my JS code a lot. I initially wrote the whole project using the 'createElement' method, but this led to having a LOT of lines of code in my index.js file because I had to set classes/additional attributes/innerText separately. About halfway through completion, I discovered that I could use the 'innerHTML' or 'insertAdjacentHTML' methods to clean this up considerably. I'm not totally sure which practice is better, but I do know that using the latter made my file a lot more readable!

Something else I ran into was having to use 'bind' within my JS classes! I was setting up Event Listeners when an object was instatiated, but because these event listeners were embedded within object methods, they were losing the execution context of the object and instead defaulting to using the window as the execution context. After much Googling, I discovered that I had to simply bind the event handlers to the context of each object in order to get these to work. I thought this was a particularly useful application of something we'd learned in this module, so it seemed worth noting here!

I still feel as though I have a lot to learn, but I am pretty happy with my project so far! If I were taking this farther, I'd also add in a password attribute for the user & expand the application so that it could encrypt the password & so forth. I'd also next like to try creating something even more interactive -- maybe building a game! That'll be one of my goals as I approach the end of this course and get ready to put together a portfolio!
