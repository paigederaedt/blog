---
layout: post
title:  "Second Studio Day*"
date:   2014-10-14 21:43:47
categories: jekyll update
---
Today was our second studio day. We started with a stand up style check in on the second floor porch. We all brought or talked about a book we wanted to share with the class. I talked about ['House of Leaves'](https://www.google.com/search?q=house+of+leaves&es_sm=119&source=lnms&tbm=isch&sa=X&ei=ddxHVJGDNajlsATuoIKwDw&ved=0CAgQ_AUoAQ&biw=1186&bih=720) by Mark Danielewski because of it's really interesting text layouts on each page. Everyone else shared some awesome books as well! 

![Book sharing]({{site.baseurl}}/assets/booksharing2.png) 

![Book sharing]({{site.baseurl}}/assets/booksharing1.png)

After this we listed to Zan demo a talk she is doing in November about Simpson's paradox. She demoed a new chart style she created with [Martin Wattenberg](http://www.bewitched.com/) to better visualize data so that this effect becomes more apparent. The paper that the talk about can be found [here](http://static.googleusercontent.com/media/research.google.com/en/us/pubs/archive/42901.pdf) 

The rest of the day was pretty standard studio...just continued to work on creating my circos visualization in d3. 

Here's a semi-finished product!:  

<iframe src="//player.vimeo.com/video/113674215" width="500" height="400" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>  

I managed to get it animated. In the background, I have the list of words that contain each letter connected to each chord segment, but I need to figure out how to display them as well when you hover over.

A few more ideas I had were:  
* for a more static visualization, be able to choose a sequence of n letters and iterate around the circle. I could maybe do this by constructing and array of letter tuple frequencies - each word will have it's own letter tuple frequency array associated with it. Then for each word, check if the selected tuple has a nonzero entry in its frequency array-->realized I need a way to access more letters so that you're not limited to tuples...??  

* have text read to you/move across screen while the circle viz is drawn out live, line by line. Maybe have ceratin lines different colors based on sentiment or define drawing motion based on sentiment. Maybe the whole visualization morphs through time based on cumulative sentiment?  

* maybe I can analyze the actual progam text in these same ways? Feed the actual code used to write the visualization as the data. I would need to account for more special characters though  

* this idea is unrelated to the circle visualization but also deals with text - dragging letters into a line but gets harder or easier to spell something out based on some rules (maybe with words instead of letters? but where to get the words?). This would investigate how programming could force you to write in a certain way - what happens?