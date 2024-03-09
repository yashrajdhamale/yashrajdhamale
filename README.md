Ryan Lanciaux
Ryan Lanciaux
Posted on Jul 16, 2020


72

17
Add a visitor count on your GitHub profile with one line of Markdown
#
webdev
#
watercooler
In a previous article, I wrote about how you could add a visitor counter to your GitHub profile with a little node/express app. The article suggested that if you wanted to add a counter to your GitHub profile, you could copy and run the code on your own server. I've recently updated this operation to be a lot easier.

Ryan Lanciaux profile imageRyan Lanciaux@ryanlanciauxtwitter logo
🚨 Add visitor count to your GitHub Profile in one line 🚨

```
![Visitor Count](https : //profile-counter.glitch.me/{YOUR USER}/count.svg)
```

☝️ in your README.md (Note: There's space around : that you will need to remove -- link was autoformatted otherwise 🤦‍♂️)
13:29 PM - 16 Jul 2020
Twitter reply action Twitter retweet action Twitter like action
You can now add a counter to your GitHub profile with the following line of Markdown
![Visitor Count](https://profile-counter.glitch.me/{YOUR USER}/count.svg)
I'd love to know what you think!

Top comments (31)
Subscribe
pic
Add to the discussion
 
 
pujux profile image
Julian Pufler
•
Jul 17 '20

I built the same thing a few days ago, hosting it on my dedicated server so it won't get any rate-limit oder downtime. badges.pufler.dev 👍


9
 likes
Like
Reply
 
 
janmam111 profile image
JanMam111
•
Aug 3 '20 • Edited on Aug 4

It looks amazing. I can advise you to use a dedicated server if you want your site to work perfectly all the time. I use intergrid.com.au/dedicated.php.au for many years, they have the best offers at the best prices. I really appreciate that they provide help and they were in general first to explain to me what exactly I needed. Try to check it, maybe you'll find it useful for your purposes. Moreover, it is available not only in one country, so it'd be useful for people from different countries.


2
 likes
Like
Reply
 
 
pujux profile image
Julian Pufler
•
Aug 3 '20

Thank you!


1
 like
Like
Reply
 
 
jdromero88 profile image
José Romero
•
Jul 21 '20

Thanks I added it to my profile!
github.com/jdromero88


3
 likes
Like
Reply
 
 
pujux profile image
Julian Pufler
•
Aug 3 '20

awesome!


2
 likes
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 17 '20

Very cool. Looks nice.

A note of potential clarification.. this is using a “boosted” server (paid feature) in glitch. There should be no downtime or rate limiting like the non-boosted tier.


2
 likes
Like
Reply
 
 
pujux profile image
Julian Pufler
•
Jul 17 '20

Oh, didn't know that, I figured it was a normal free glitch instance like the one that went more or less down. Cool!


2
 likes
Like
Reply
 
 
rahuldkjain profile image
Rahul Jain
•
Jul 17 '20

Tired of updating GitHub profle README with latest features again & again?

If yes, then I have developed a tool to do the same for you in just 1 click 🤓

🚀 Try the tool: live tool

If you find the tool useful, show some love by giving a ⭐ on github repo
GitHub logo rahuldkjain / github-profile-readme-generator
🚀 Generate GitHub profile README easily with the latest add-ons like visitors count, GitHub stats, etc using minimal UI.
GitHub Profile Readme Generator

GitHub Profile README Generator
github-profile-readme-generator licence github-profile-readme-generator forks github-profile-readme-generator stars github-profile-readme-generator issues github-profile-readme-generator pull-requests join discord community of github profile readme generator

github-profile-readme-generator gif

View Demo · Report Bug · Request Feature

Loved the tool? Please consider donating 💸 to help it improve!

sponsor github profile readme generator Buy Coffee for rahuldkjain Buy Me A Coffee

Tired of editing GitHub Profile README with new features? This tool provides an easy way to create a GitHub profile readme with the latest add-ons such as visitors count, github stats, etc. 🚀 Demo 
Try the tool: GitHub Profile README Generator

🧐 Features
Just fill in the details such as Name, Tagline, Dev Platforms Username, Current Work, Portfolio, Blog, etc. with a minimal UI.

Uniform Dev Icons

Uniform Social Icons

Visitors Counter Badge

GitHub Profile Stats Card

GitHub Top Skills

GitHub Streak Stats

Dynamic Dev(.)to Blogs (GitHub Action)

Dynamic Medium Blogs (GitHub Action)

Dynamic Personal Blogs from RSS Feed (GitHub Action)

Wakatime Stats contribute

Buy Me A Coffee button

Click on Generate README to get your README in markdown…

View on GitHub

9
 likes
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 17 '20

Cool.


1
 like
Like
Reply
 
 
vikramkadiam profile image
Vikram Kadiam
•
Jul 18 '20

Hey Rahul, that's a pretty useful tool.It looks like the visitor counter is counting even the browser refreshes from same user.Is this expected?


1
 like
Like
Reply
 
 
rahuldkjain profile image
Rahul Jain
•
Jul 18 '20

Yes because its visit-count not unique-visit-count


1
 like
Like
Reply
 
 
king11 profile image
Lakshya Singh
•
Jul 16 '20 • Edited on Jul 16

There was another provider with same service named visitor-profile-badge, It recently stopped working and I was left with no other option other than to just remove it. I hope your application is there to stay :) because it's not good that you make something it stops working cause of server or other load.


3
 likes
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 16 '20

I was not aware of that one. I have no intent on removing this one :D


2
 likes
Like
Reply
 
 
jonrandy profile image
Jon Randy 🎖️
•
Jul 17 '20

Seems to add page views - pretty different from a real visitor count. Hit refresh, the count goes up


1
 like
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 17 '20

Refresh is a new view of the page :) it’s working as intended


1
 like
Like
Reply
 
 
jonrandy profile image
Jon Randy 🎖️
•
Jul 17 '20 • Edited on Jul 17

So, this is also a new view of the page! 😄
curl https://profile-counter.glitch.me/{YOUR USER}/count.svg

2
 likes
Like
Thread
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 17 '20

Curl is pretty cool 👍


1
 like
Like
Thread
 
jonrandy profile image
Jon Randy 🎖️
•
Jul 18 '20

You'd be better off checking the referrer to make sure the image was loaded in the context of the page where the counter is. Otherwise, you're just counting 'loads' of that image - wherever they may have come from


1
 like
Like
Thread
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 18 '20

A referrer check would work in many contexts, however, the primary intent of this project is for use on GitHub. GitHub has a caching later that prevents tracking docs.github.com/en/github/authenti... - this is a “for fun” project that I made quickly in hopes people would have fun with it on their GitHub profiles. If this were a commercial product or an analytics package that was not for use on GitHub, I would check the referrer among other things.

If you are interested in making changes (as a new project), the code is available in the prior article mentioned above (noting there is no database in that version)


4
 likes
Like
Reply
 
 
olton profile image
Serhii Pimenov
•
Jul 17 '20 • Edited on Jul 17

this script increase counter on each hit. you can wind up the counter by reloading the page to insane indicators!


2
 likes
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Jul 17 '20

So you're saying it works? :D Each time you reload the page it counts as a new visit. This is partially due to every visit coming from GitHub's camo caching layer (no way to tell if it's a repeat visitor since they are ALL repeat visitors).


5
 likes
Like
Reply
 
 
gayanvoice profile image
Gayan Kuruppu
•
Jun 7 '21

I created this GitHub Action that uses GitHub API. It updates daily and does not require any servers or databases. It automatically saves changes into the repository. Go to the template GitHub Insights Template


1
 like
Like
Reply
 
 
rahuldkjain profile image
Rahul Jain
•
Jul 18 '20

Considered


2
 likes
Like
Reply
 
 
ljnce profile image
Luca
•
Aug 6 '20

Thank you Ryan, easily way with awesome result!


2
 likes
Like
Reply
 
 
ryanlanciaux profile image
Ryan Lanciaux 
•
Aug 6 '20

Thanks for the kind words! Glad it works out for you :)


2
 likes
Like
Reply
 
 
princemuel profile image
Prince Muel
•
Jul 31 '21

how do you insert the {your user} variable?


1
 like
Like
Reply
 
 
ng_update profile image
Kieran
•
Jul 17 '20

Coolio!!! Got it up and running in no time! (had to create the repo as referenced in dev.to/m0nica/how-to-create-a-gith...)

Thanks!!!


1
 like
Like
Reply
 
 
nirbhayvashisht profile image
Nirbhay Vashisht
•
Sep 24 '20

It is awesome. Thanks


1
 like
Like
Reply
View full discussion (31 comments)
Code of Conduct • Report abuse
profile
Platform.sh
PROMOTED

Billboard image

Experience effortless application deployment 🚀
Deploy your apps seamlessly on an all-in-one PaaS.
🚀 Flexible, automated infrastructure provisioning.
🎯 Multicloud and multistack.
👾 Safe, secure and reliable around-the-clock.
👉 Get a 30-day free trial to build and deploy your way.

Claim your free trial

Read next
devendra_2806 profile image
JavaScript Loops: A Beginner's Guide
Devendra Devendra - Feb 18

digital_hub profile image
WordPress 6.5 Beta 1 is ready for download and testing!
hub - Feb 14

ben profile image
Meme Monday
Ben Halpern - Mar 4

syedmuhammadaliraza profile image
Next js with Axios Data Fetching
Syed Muhammad Ali Raza - Feb 27


Ryan Lanciaux
Follow
Hi 👋 I'm Ryan Lanciaux. I love web and mobile application development. In my freetime, I create electronic music.
LOCATION
Somewhere.
JOINED
Sep 24, 2017
More from Ryan Lanciaux
A couple tips for working from home
#watercooler #productivity #remote #tips
Better testing with Storybook
#react #webdev #testing #javascript
Optional Chaining in JavaScript
#webdev #javascript #tutorial #beginners
Clerk
PROMOTED

Authentication & User Management: Powering the Modern Web
Clerk image

Streamline app authentication and user management with Clerk. Quick setup for React, Next.js, and modern frameworks. Customizable UI components for sign-in, sign-up, user profiles, and organizations.

Start building for free

![Visitor Count](https://profile-counter.glitch.me/{YOUR USER}/count.svg)

# Introduction
Welcome to my GitHub page! Here, you'll find a collection of projects I've developed, ranging from web development to data structures and algorithms implementations. As an engineer, I'm dedicated to creating practical solutions that address real-world challenges. Feel free to explore my projects and don't hesitate to reach out if you have any questions or feedback!

# About Me
I am an engineer with a passion for innovation and problem-solving. My journey in the field of technology has equipped me with skills in HTML, CSS, JavaScript, DSA (C++), and React.js. With each project, I strive to push the boundaries of what's possible and learn new concepts along the way.

# Skills

| NO   | SKILLS       |
|-----:|--------------|
| 1    | HTML         |
| 2    | CSS          |
| 3    | JavaScript   |
| 4    | DSA (C++)    |
| 5    | React.js     |

---
> Keep Working
