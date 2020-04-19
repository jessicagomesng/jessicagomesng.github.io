---
layout: post
title:      "CLI Gem Project"
date:       2020-04-19 08:41:36 -0400
permalink:  cli_gem_--_first_project
---


Wow!! I've finally finished this project! I don't even know where to begin with this blog post...

![](https://scontent-lhr8-1.cdninstagram.com/v/t51.2885-15/sh0.08/e35/s750x750/91984740_524425668501196_7969765844103512120_n.jpg?_nc_ht=scontent-lhr8-1.cdninstagram.com&_nc_cat=104&_nc_ohc=hnkbBuk5UjQAX_DU6O4&oh=31cd2c57048bbcf10d969199e76b3868&oe=5EC658D6)

When I first read about this project, I was immediately daunted by everything -- it just seemed like there was suddenly so much information that I had to digest. There are so many resources out there that I think it can sometimes feel really overwhelming to be presented with all of them!! I also had no idea what to scrape or what to make my CLI  about.  I was sitting inside with my dog Peety (pictured above) & my husband talking about the project when we started talking about how much we adore Peety and having a pet, and, from there, I decided pretty much right away to use a CLI to access info from an animal shelter page!

I was initially going to scrape data from the Battersea shelter here in London, but my project manager emailed me to let me know that the site was too slow to use Nokogiri, so I ended up going with the Blue Cross pet shelter instead. 

Honestly, I learned *so* much from this project. It was really helpful to me to read over a lot of the resources, and, in particular, it was useful for me to watch Avi Flombaum building the Daily Deals CLI gem. I had a much better understanding of how to go about building my CLI in a step-by-step fashion, and I felt a lot less overwhelmed once I knew the process I should be going through. It was also really useful to hear him talk about the importance of researching the things you're doing and making sure you have a complete understanding of everything before you move forward. I think it can be easy to get caught up in just zipping through everything and completing labs rather than taking my time to get to understand a concept, so it was good to be reminded of this, and it really made me dig deeper into understanding using bundler & gems (which, to be honest with you, I didn't fully get before this project...and there's still so much I have to learn!) 

Writing the code for this turned out to be probably the most straightforward part of the assignment. I still don't know if the code is presented in the most elegant manner -- when I look at it, I want it to be simplified even more; however, I did spend quite a long time trying to strip it down and making sure it wasn't too repetitive. I'm sure there are many other ways to make it even more efficient.

I actually found the hardest part of this to be turning the project into a gem to publish to RubyGems! This truly taught me soooo much about the way gems work -- I don't think I fully grasped gems at all until I was faced with this challenge. I initially was just using 'gem build' and then trying to publish my gem straight to RubyGems, but I was running into all sorts of problems because of the way my gemspec & require statements were set up (they were set to their defaults from running bundle gem, and so the gem that was built into my project directory was being required meaning the gem was requiring itself...there were so many road blocks I ran into, haha). This took sooooo long for me to really fully understand -- I read so many guides and spent so long just trying to test out my gem without receiving a LoadError. The good news is, after hours (!!) of poring over random StackOverflow queries and guides to publishing gems, I think I finally gained a clearer understanding of what was going on and was able to publish my gem! I even got my sister in New Zealand to download it and test it out, ha ha! 

This was a very, very useful project for me. There were basic concepts like '.' and '..' in the command line, as well as using 'require' / 'require_relative', that I just initially glossed over until I started down the rabbit hole. I even started writing my own tests so that my gem could be published! (I honestly mostly mimicked the framework for these tests from previous labs, like the Student Scraper one, but it still gave me a deeper understanding of how to write these & how these work) I'm grateful the project is finished now and that I'm able to move forward learning more concepts, but I'm also very glad to have had the opportunity to apply my learning to something new! I had a lot of fun!

