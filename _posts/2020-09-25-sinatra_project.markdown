---
layout: post
title:      "Sinatra Project"
date:       2020-09-26 02:44:47 +0000
permalink:  sinatra_project
---



This project pushed me in so many different ways. It’s incredible how I can enjoy something that causes me to break down in frustration so often. I can honestly understand what a love/hate relationship is now that I’ve gotten into coding. And I’m going to be completely honest here, I thought this project was going to end me. 

To start, I was overwhelmed. Self doubt is my worst enemy and it nearly beat me. However, I am also an annoyingly optimistic person. So, to help ease the pain of this project build I decided to have this center around a passion of mine. Art. 

I’ve built a site where artists can submit lists of supplies that they own. As an artist myself I have moments where I’m going through my hoards of paints, pencils, markers, etc. and stumble upon something that I had completely forgotten I owned (granted this may just be a hoarder issue on my part…). So I wanted a place to be able to easily see a list of supplies that I own. 

I had to make myself look at this step by step because otherwise looking at everything I needed to do was incredibly overwhelming. Bite sized pieces. Start off with running the Corneal gem(a lifesaver honestly) and it created a nice little skeleton to work off of. Then created my models to establish the has_many and belongs_to relationships. 

I hit a roadblock early on that held me back for a couple DAYS (another thing coding is teaching me is that it is okay to ask for HELP). I could not get my list of supplies to populate on the Supplies index page. Turns out it was a syntax error.  I had missed adding the method=“POST” in my new.erb file. 

`<form action="/supplies" method=“POST”>`

From there it was smooth sailing for a bit until my routes were getting messed up. Some were working, whereas others weren’t. Sinatra kept acting as if there was no route to connect with. After hours of looking over my code with a couple cohort friends and an instructor we had discovered that in my supplies_controller I had written the code as:
 
`redirect to ‘/supplies/#{@supplies.id}’`

Instead of 

`redirect to “/supplies/#{@supplies.id}”`


The little details matter in coding, even with something so small as the specific quotation marks used. It had to do with string interpolation. These quotes “” let you substitute the result of the code into the middle of a string where as ‘’ do not. 

Overall I learned a lot from this project. More than anything I learned to not rush things and to ask for HELP. I have so much to learn but I look at what I’ve built and it doesn’t look like a totally unreadable language which is a huge win for me. Despite all the frustration and tears I can honestly say I’m excited for the next project! 
