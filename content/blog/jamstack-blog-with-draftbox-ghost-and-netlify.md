---
title: 'JAMstack Blog with Draftbox, Ghost CMS,  and Netlify'
date: Fri, 22 May 2020 13:01:35 +0000
draft: false
featureImage: images/blog/Jamstack-with-Draftbox-Ghost-and-Netlify-1024x576.png
postImage: images/blog/Jamstack-with-Draftbox-Ghost-and-Netlify-1024x576.png
tags: ['Blogging', 'draftbox.co', 'Heroku.com', 'Netlify', 'Web Development']
---


Create FREE JAMstack blog with Draftbox, Ghost CMS & Netlify CDN

I had been running my blog [ontraveldiary.com](https://ontraveldiary.com/) on WordPress for a year, and I must say WordPress is an amazing platform and it is evolving with time to provide better features for bloggers. But at times it becomes an overkill for a simple blogger like me. Trying my way around a number of plugins to achieve a certain goal, I always felt that it would have been better if there was one CMS which didn’t involve so much technical knowledge (trust me you need more than enough technical no-how to get around WordPress, though it is a code free platform for a larger part).

Another issue I constantly faced was SPEED of my blog. No matter how hard I tried (I mean I tried a number of **caching plugins, image optimization techniques, HTML, CSS & JS minifiers, inline critical CSS**), I always ended up with more than 8 Seconds of loading speeds on gtmetrix.com. I know, it is not entirely WordPress’ fault and the theme, plugins & assets had a lot to do with it. Then in order to survive running a custom blog on WordPress one must also know her/his way around servers. I mean how many times have we encountered errors that can only be resolved in the back-end. The most common errors like:

**Stuck In Maintenance Mode After Update**

**Error Establishing a Database Connection**

**500 Internal Server Error**

If you are facing any such errors please visit this link **https://pressable.com/2018/04/17/7-common-wordpress-errors-and-how-to-fix-them/** and resolve it. It takes significant efforts, time and technical acumen to solve these errors. One needs to be acquainted with C-panel or back-end technologies to resolve such errors and restore the WordPress blog/website.

### The Search for Something Better

I felt that blogging must be simple, should not involve doing too many things (technical things). On the contrary, blogging must be focused entirely on content.

That is when I decided to look towards JAMSTACK blogs and convert my blog into JAMSTACK blog. If what I had learned through my research on Google and YouTube, JAMSTACK must make my blog faster, should bring down the involved cost of running a blog, and above all, should make my blogging life easier.

What is JAMstack - Is it the future of websites?
------------------------------------------------

As defined on the official website of JAMSTACK ([www.jamstack.org](http://www.jamstack.org)) -

> “Fast and secure sites and apps delivered by pre-rendering files and serving them directly from a CDN, removing the requirement to manage or run web servers.”
> 
> From the torch bearers of Jamstack

### Benefits of Using JAMstack

*   Better performance - I mean really, super speed.
*   Higher security - With a static site in the front and headless cms in the backend, what better way to shield your data.
*   Cheaper & easier scaling - just connect CDNs and load balancing and you are good to go
*   Easier Developer’s life - Yep! No more fiddling with alien plugin systems (but you still need to remain a developer)

What better future can you dream of? I know “SKY has no limit”. But ask any developer today, and they will vouch for JAMstack’s future.

> Javascript & Jamstack are the technologies of the future.
> 
> I strongly feel this.

### Is JAMstack for a non-techie blogger?

The definition of JAMstack on its official website does make it sound very easy. But this definition doesn’t help you get up and away with JAMstack at all. You need something more than this definition. There is a SSG (Static Site Generator) like Gatsby, Hugo, Jekyll, Nuxt and numerous others (again technicality involved) - which generates a static site for you, then you need a headless CMS to control your content, and finally your way around the CDNs like Netlify to get your blog up and running (and I thought JAMstack was going to solve all my problems).

If you are not a technical geek, you are going to regret deciding DIY (Doing it Yourself) your jamstack website/blog. JAMstack only solves the issues with speed and provides you with modern features of the evolving digital world such as [AMPs](https://amp.dev/) (Accerlerated Mobile Pages) & [PWAs](https://web.dev/progressive-web-apps/) (Progressive Web Apps). But it never removes the need for technical knowledge. In fact it requires more technical knowledge to start your blog than to maintain it. You are better off blogging on wordpress.com (entirely different from wordpress.org), blogspot or medium.

The Solution - Draftbox - The SUPER CMS
---------------------------------------

![Draftbox logo](https://kesaviweb.com/wp-content/uploads/Draftbox-logo.png)

Draftbox - New Age Blogging

Draftbox is a new age blogging platform built on “Gatsby” that leverages the JAMstack technology and makes it easier for non-techies to benefit from futuristic JAMstack technology. Read more about it on its official website [www.draftbox.co](https://draftbox.co/). It is still under continuous development and beware you might find glitches here and there (no glitch in their support though), but it surely eliminates the need to learn Nelify, Github and Static Site Generators.

As of now, Draftbox supports WordPress & Ghost as headless CMS for deploying JAMstack blogs. The Draftbox team is also working on bringing JAMstack sites into their folds which, as claimed by their team, is under active development and should be launched anytime soon.

As per latest update, draftbox works as an independent CMS for blogging and you can manage your posts right inside draftbox.co.

For those planning to migrate their blogs from **WordPress or Ghost CMS** to **JAMstack**, Draftbox automates the process within a few clicks and makes the whole experience enjoyable.

### JAMstack Blogging with DRAFTBOX in TWO SIMPLE STEPS

I moved my WordPress blog to ghost and turned it into a JAMSTACK blog using draftbox. In this article I am going to share my journey. It involves no cost as everything is built using free tiers and should help anyone start a custom blog at zero cost. Hope it helps you.

To follow this journey with me you will need to create a free account on [heroku.com](https://heroku.com) (for Ghost CMS), & [Netlify](https://www.netlify.com/) (great if you already have one). And of course you will also need an account on Draftbox. Go ahead and create a free account on [www.draftbox.co](https://draftbox.co) to follow along.

#### **Step 1. Deploying GHOST CMS on Heroku**

First of all, visit heroku.com and create a free account. Once successfully logged in, you will need to deploy and configure Ghost CMS using SNathJr’s one-button heroku deploy for Ghost 3.2.0 by visiting [https://github.com/snathjr/ghost-on-heroku](https://github.com/snathjr/ghost-on-heroku) (there are other versions as well such as cobyism’s but those have outdated Ghost installations). Scroll down the page and find the **“Deploy on Heroku”** button.

![](https://kesaviweb.com/wp-content/uploads/Deploy-to-Heroku.jpg)

Click this button on the page to deploy Ghost on Heroku

Once you click on the “Deploy on Heroku” button, you will be taken to the page as shown below to create a new app on heroku.com (if already logged in):

![](https://kesaviweb.com/wp-content/uploads/deploying-ghost-cms-on-heroku.jpg)

New app creation on heroku.com

Provide a name for your app and copy paste the same name into **“APP\_PUBLIC\_URL”** replacing **“YOURAPPNAME”** (this step is essential and can’t be skipped as it would lead to 404 errors in your blog). See the example as shown in the screenshot below:

![](https://kesaviweb.com/wp-content/uploads/providing-app-name-and-app-public-url-in-heroku-app.jpg)

setting up a new app on heroku

After you are done, just click on the **“Deploy app”** button and the rest of the process is automated. It takes a while and you will be shown that _“Your app was successfully deployed”._ Click on the **“View”** button to go to your ghost admin panel and follow along. See the screen recording below:

Setting up Ghost CMS for first use

#### **Step. 2. Connect Ghost CMS with Draftbox**

Go to [www.draftbox.co](http://www.draftbox.co) and create a free account. After successful login, you will be greeted with a “Draftbox Wizard” that will help you connect your ghost blog to Draftbox and also host a static front end on netlify (you must have a netlify account). Follow along as shown in the screen recording below (In case you get stuck or the build fails, you can chat with Draftbox's team right inside the wizard):

Setting up Blog on Draftbox

After the wizard has successfully published your static front end on Netlify, all that you need to do is integrate Draftbox with Ghost CMS with **_webhooks_**, so that whenever you create a post on ghost or change any other settings, it gets updated on the front end. Follow the screen recording below:

Integrating Ghost CMS with Draftbox using webhooks

**Hurraayyyyyyyyy!!!** You have successfully created a Jamstack blog using the magic of Draftbox in **just 2 Simple Steps**. Now you can entirely focus on blogging and Draftbox's team will take care of everything else. Draftbox's team analyzes your published/production blog’s performance and if there is anything to improve they immediately inform you, so you don’t lose out on any aspect.

#### Blazing fast performance with AMP & PWA

Draftbox provides your blog with a blazing fast front-end built with Gatsby JS. It comes with an added advantage of AMPs (Accelerated Mobile Pages) & PWA (Progressive Web Apps) for your blog. I checked my blog's performance on gtmetrix.com after migrating to JAMstack with draftbox and I was amazed to see the results.

![gtmetrix speedtest result for ontraveldiary jamstack blog](https://kesaviweb.com/wp-content/uploads/gtmetrix-speedtest-result-for-ontraveldiary-1024x482.jpg)

Wow!! Draftbox made my blog Blazing fast!

#### Handling Contact Forms and Subscriptions with Draftbox

Draftbox makes handling contact forms and subscriptions ridiculously easy. Just go to the “Forms” tab to see all Contact Forms and subscription form submissions you have received via your blog.

#### Extra Perks with Draftbox

As soon as you have your JAMstack blog deployed using Draftbox you get additional features from them. You can integrate your **Google Analytics** account with your blog and analyze the traffic as usual. You can also integrate **Disqus** comments on your blog by simply creating an account with Disqus and copy pasting “short-name” into Disqus setting under **“Integrations”** tab in the dashboard.

#### Future Updates from Draftbox

As updated by the Draftbox;s team, they are working on integrating many other functionalities inside Draftbox dashboard such as Adsense, Auto-posting on Social Media Platforms (suggested by us), email delivery of form submissions and subscriptions and many many more. Currently they are constantly updating their platform.

We are very hopeful of Draftbox and expect it to come out with more exciting features which make the life of a blogger easier.

If you are not a big fan of reading into lengthy blogs, watch the video below and follow along. Like the video if it helps you and subscribe to our YouTube channel to receive updates on more such videos.

[![Video guide to create JAMStack blog with draftbox](http://img.youtube.com/vi/Rg1P4fr6mzw/0.jpg)](http://www.youtube.com/watch?v=Rg1P4fr6mzw "JAMStack Blogging with Draftbox")

Free JAMSTACK Blog with Draftbox, Ghost CMS, Heroku & Netlify CDN