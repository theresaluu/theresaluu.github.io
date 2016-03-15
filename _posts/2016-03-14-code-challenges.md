---
layout: post
title: "Tackling Code Challenges"
categories: interviewing, datatypes, tips
excerpt: Lessons learned doing consecutive code challenges.
---

We've all been there.  Me?  I'm still there.  I've been working on consecutive code challenges, looking for my next professional adventure as a web developer. Today, though?  Today: I finished one I had built up so much anxiety about. 

__Current mood__: Beyonce-Crazy-In-Love-Video!

Reflecting on this current series of completed code challenges:

### Things I've Done Right
**1. Be very honest with companies I've been interviewing with about what I have on my plate**
  Potential employers are very receptive to your needs especially if you have been authentic in your interactions with them since the beginning.  Whether you have limited time because you are job-hunting while employed or juggling multiple assignments from multiple companies, let them know upfront about your time constraints.  So far out of six code-challenge-giving companies, only one of them gave me a hard time for trying to be upfront about when I could start on their assignment.  You can't be a good fit with everyone.

**2. If a company gives you multiple challenges, do not try to divide the given time you have to complete the tasks by the number of tasks given**
  Mathematically, this sounds it would be a good idea to give each coding assignment 4 hours if you have 2 challenges and 8 coding hours available to you.  Each time I've encountered a multiple-challenge situation, I've dove into the first one with as much gusto as I had: tested, refactored, meeting my 80-character-per-line self-imposed requirement, extracting functionality from giant methods into many tiny ones.  Have I ran out of time and not completed the second assignment?  Yes, and I just proceeded to inform the person assigning me the challenge.  I've had mixed reactions but all of them have been positive.  Once, I hadn't run out of time but I turned the first assignment in, telling them I was going to start on the second one.  My code was solid enough that they told me I didn't have to complete the second one.  Another time, I completed the first assignment just in time for the interview.  During the interview, I was able to speak to my code sample and talk them through my implementation well enough that they said I was invited to finish my second code challenge but I didn't have to.  When I went home, I decided to give it a try.  While the first assignment took me about 4 hours, the second one took less than five minutes, including the time it took me to google a SQL question.

**3. Use Pry!  Your console is not good enough**
  Your objects may not be behaving the way you think they are.  I was doing some work with date ranges as params and the queries that I put in console were working fine.  My data looked just as it should've; however, my specs were failing, and I didn't understand why until pry was telling me what would information was actually returning.

### Lessons Learned
**1. This is not the time to try out numerous new gems/databases/frameworks you've never played with before**
  I not only wanted to demonstrate my knowledge, but I also wanted to demonstrate that I could learn really quickly, too.  My decisions were not based on the project requirements.  I chose my paths myself.  Professionally, at RED Digital Cinema, I was working with a Rails 3 stack with a mongoDB with test unit in place and exposure to coffeescript, jQuery, and rabl.  In one challenge, I tried a Rails 4 app in postgres using mini-test and shoulda-matchers with guard.  That wasn't that huge of a deal as when I tried to build another app as a rack app, which I wasn't sure how to test effectively so then I built a sinatra app, but then I was tempted by Rails 5 in beta (for their Rails API gem integration).  I ended up just using Rails 4 with a manual inclusion of the rails-api gem, RSpec, sqlite3, and jbuilder.  Needless to say, my tool-analysis-paralysis was a huge time suck.  I have resolved to respect my own time and that of those who are going to review my code to try to keep the "new toys" to a minimum in a code challenge.  I still do want to build a rack app but I'm going to do it on my own terms/time.

**2. Time vs DateTime**
  I was storing dates with time as Time.  I was able to call Time.now.iso8601 and compare it to other times given- no problem in console.  As mentioned above, I used pry to find that my queries against the objects with this Time attributes were responding only with the correct time but with the incorrect date: Jan 01, 2000.  It turns out that Time will store your date correctly (that is why console didn't show any errors when I was testing my time comparisons), but it won't return your date correctly when queried.  My solution was to write a migration to change that datatype to DateTime instead of Time.

**3. My READMEs can always use a little more love**
  Several of my assignments have asked for instructions in the readme, and since doing them, I don't think I'm going to go back to the couple-a-liner READMEs.  These are like the eyebrows of the repo: they can make or break the first impression.  If any of you have some rad READMEs to point me to, I'd love to see recommendations to tailor my own README style.

These challenges have made me a better developer, and as taxing as they are, they do provide small wins in this complicated dance that is the developer hiring process.  Best of luck to you all out there trying to find your "good fit"!

-t
