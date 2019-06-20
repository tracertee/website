# How did this go down?

This readme is for me as much as it is you.  I spent the better part of a day trying to figure jekyll and git pages out. So here is my first writeup!


## Installation

1. Go get a github account then follow the instructions on how to build Pages [here](https://pages.github.com).  I chose the <i> Leap Day </i> theme

2. Follow the tutorial to figure out how the hell <i> Jekyll </i> works [here](https://jekyllrb.com/docs/step-by-step/01-setup/)

3. The reference material for the <i> Leap Day </i> theme is [here](https://jekyllrb.com/docs/step-by-step/01-setup/)

4. Once you get it working on your local machine, I copied: <br>`<jekyll root>/_layouts/default.html` <br> and created my own layouts based on the templates that I woudld be doing.  So for the CTF stuff, I had the following:
* challengeList.html  
* ctfList.html  
* writeup.html
* default.html  <br><br>

5. This way I would have a template to list the challanges (challegeList.html), a template for listing the ctf's (ctfList.html), a template for writeups (writeup.html), and the default. 
Each template has a bit of code in it as you can see on github to iterate through lists and populate tables.  The default is a nice blank page with just the title.  This took a bit of time fucking around with the ruby based for loops.  

6. The way I ended up organizing this (keep in mind I am a hacker not a professional programmer) was to use the "categories" variable in the 'front matter' to differentiate between a ctf competition and a ctf challenge.  All CTF competition will get the "list" name and all challenges for that ctf will get the "<name of the ctf>" as their categories name.  From there I iterate on the respective layout to populate the tables with 'posts'.  Everything is a post (meaning ctf comptitions and challenges are both posts).  I organized everything in the directory structure: <br>

`<jekyll root>/_posts/competitions/<ctf name>/<post in jekyll format>`

7. I created a 'post' template for the writeups and for the competitions so I wouldn't forget this complicated shitshow.  The end for now...



