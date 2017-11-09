---
layout: post
title:  "Robots, Humans, Comments, and Open Graph"
comments: true
---
# What is robots.txt and how have you configure it for your site?
The robots.txt file gives instructions about the site to web robots. Web robots are programs that search the web automatically for information. They have many different uses, but can for example be used by spammes to scan for email adresses.  
I decided to allow robots from Google, but from no other site. I placed the robots.txt in my src file and wrote:  
    *User-agent: Google*  
    *Disallow:*  
    *User-agent:*  
    *Disallow: /*  
# What is humans.txt and how have you configure it for your site?  
Humans.txt is a text file containing information about the site and the people - authors - behind the web site.  
I included information about the team, i.e. me, and the site. I placed the txt file in the src file, and added the **humansTXTbutton** with a link to the file in the footer of every page and post. You can find it at the bottom of this page, under my email adress.  

# How did you implements comments to blog posts
I used Disqus to implement comments on my blog posts. Disqus is a blog comment hosting service for websites.  
I created an account, installed Disqus and icluded the html for disqus comments on all the blog posts. 
# What is Open Graph and how do you make use of it?
Open Graph is a technology that makes it easier to share websites or pages on social media, such as Facebook. With Open Graph meta tags you can identify what you want to show when the page is shared.  
I implemented meta tags for title, type, url and image in the head of the website. 

{% if page.comments %} {% include disqus_comments.html %} {% endif %}
