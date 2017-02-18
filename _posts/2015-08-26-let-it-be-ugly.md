---
layout: post
title: "Let It Be Ugly"
categories: tech
excerpt: If you love something, then let it go.  And if you **fucking hate something** but it's code you are working on, you also have to let it go ...
---

If you love something, then let it go.  And if you **fucking hate something** but it's code you are working on, you also have to let it go ... live online while you keep iterating on it 'til it stops looking like a bastard.  Why not make my first post be a declaration of roadblocks?

My current roadblocks are as follows: 

1) **Rubynista.com is currently being transferred from Hostgator to Google Domains**

Why?

I do not need hosting service because I am using gh-pages + Jekyll to build this blog.  This is free, uses a tool I love, and gives me green squares on my GH profile- all great bonuses.  So I canceled my hosting with them and only kept the domain with them.
Only then did I discover that I would have no obvious way to delete my CNAME, and configure an A record so that I could have my blog be www.rubynista.com instead of theresa.rubynista.com.  The Rubynista does not want a subdomain with her real identity in it.

After waiting over 8 hours for a response to my "how to" support ticket, I decided it was time to move on.  It was the last straw.  I haven't had service I really cared for even before this incident.  

When I called to cancel hosting, I was on hold for 20 mins before they made me speak to two different people even though I selected "cancellation" as my automated choice even before I was put on the 20 min hold.  Twice I tried to chat with their support and after I filled out my name and domain information, I was directed to a blank page.  If your business is internet-related, these wait times and practices are out of the question.

I'm done with Hostgator.  If they delay or deny the request to transfer to Google Domains, they will need to cover themselves in the Twitter shit-storm I'm going to unleash upon them.

2) **Redcarpet Markdown included in Jekyll thinks '<!--more-->' should be rendered and is affecting my 'excerpt-separator' settings**

Original goal: Personalize each post's excerpts so that it isn't the default first paragraph of each entry.  Sometimes a girl does not want to reveal that much.

The documentation said to "include excerpt-separator: <!--more-->" in the Front Matter of your post and the excerpt would be cut off anywhere in the content of your post at the mention of <!--more-->.  

The separator, itself, would not render because it is the comment-out syntax of html.  Well, I am not using any modifiers on these separators, and they are showing up in the body of the content as well as not functioning to cut off the excerpt.

I've tried two different workarounds but they do not seem to be working with my set up.  Maybe I have a newer version of redcarpet.  Maybe there is another markdown language that would be better.  

This feels more like a problem to solve on the weekend. 

*To show you how much I am embracing this "deploy early and deploy often" approach, my list ends here: on an even number of bulletpoints.  During my first job out of college (at a design firm), I learned that it is considered "modern" to group things in odd numbers, and I have always prided myself on being a modern woman, but mantras are mantras*.

This blog will be a balancing act of building out features and design elements while maintaining a dialogue that is true to my experience.  I will take screenshots to track my building progress, and I will keep myself uncensored to accurately portray my struggles and my wins.  
  
