---
layout: post
title:      "Enter your title here"
date:       2020-10-22 01:56:08 +0000
permalink:  enter_your_title_here
---


This rails project really opened my eyes to what I can potentially build. With coding I doubt myself constantly about what I'm capable of but building but this app really helped me realize my potential! 

One of the methods I really enjoyed building was the scope method. I loved that I could build an option to have my users determine if they had been to a certain destination or not. I started with building the scope method in my destinations_controller.rb

```
def visited
     @destinations = Destination.visited 
     render :visited
    end 
```

From there I established it in my destination.rb model. 

```
scope :visited, -> { where(visited: true) }
```

After that it was just implementing the correct code in my view form. 

```
<label> Have you been here before? </label>
    <select name="visited"> 
    <option value="yes">Yes</option>
    <option value="no">No</option>
     </select>
```

With these few steps I not only have created a way for users to diferentiate where they have and haven't been and a place for them to view all the destinations they have been to! 

I know this isn't much but for someone like me who didn't even know what VS Code was two months ago, I'm proud of my growth and I'm very excited to see where I go! Especially since the world of coding doesn't seem to have a limit. Something new is always being created and maybe I can be one of those creators one day. 
