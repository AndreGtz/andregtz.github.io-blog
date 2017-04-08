---
layout: default
comments: true
title:  How To Actually Build Your Awesome Website For $15
date:   2017-03-17 16:16:01 -0700
---
{{page.url}}
{{page.url | absolute_url}}

# {{page.title}}


You are an entrepreneur, a professional looking for job or maybe you need a simple website.

This tutorial applies to static webpages, if you have a web app, then you actually need more money.

If you want a blog, then this tutorial is not for you, it can be done with the same budget but it needs a whole tutorial on its own. Maybe I will make a tutorial for that later.

If you have looked around, there are a ton of options and you can end up spending about $200 on your website.

Here I will show you step by step, how to do it spending as little as 15 dollars.

# Who is this for?

I wrote this tutorial with non-developers in mind.

If you are a developer/programmer/designer you don't need to read all the tutorial. Go for the sites that I recommend and you can figure out everything else.

Otherwise take your time going through each step.

I'm going to try my best to explain everything so anyone can do it.

If you have any question regarding this tutorial you can tweet me [@blodvodhr](https://twitter.com/blodvodhr) or opening an issue on [https://github.com/AndreGtz/blog/](https://github.com/AndreGtz/blog/)

# Let's get started: Adquiring your Domain name  

A domain name is the web address that points to your website.

You can find a lot of sites to register your domain name by searching "domain name" on google. 

I'm going to explain how to register your domain with GoDaddy. Because it's my preferred choice and it has a good international covegare. 

In Godaddy you can get a .com domain for 15USD per year.

To begin with use their search tool to find if your name is available, I'm going to search for *mypage*:
<iframe src='https://gfycat.com/ifr/ImperturbableScrawnyDamselfly' frameborder='0' scrolling='no' width='640' height='357' allowfullscreen></iframe>
Which returns all domains available for "mypage" or a little variation of "mypage".

## Which one is the best?  

.com is the most used domain, smartphones tend to have a special key [.com], and most people will add a .com when browsing for your site. 

You can come out with clever domains like: make.it , which is more creative than makeit.com.

If you are making your personal page with your portfolio in it, you can use myname.me.

There are a ton of domains, search the list of posible domains and pick the one you think fits better your purpose.

As a recommendation first buy .com, and if you  like others buy them as well.

If you go for make.it, make sure to buy make.com and/or makeit.com. So if people enter those domains you can forward them to your domain make.it.

## Register your domain  

So you have picked one (maybe more), now you will need to register an account on godaddy and give godaddy your full name, address, phone number, etc. 

This info will be public if people request the WhoIs for your domain name. Godaddy offers to hide your information for about $8. 

If your privacy concerns you, go ahead an pay for it, otherwhise just take note that your info will be exposed on internet.

<iframe src='https://gfycat.com/ifr/FreshAdorableKitfox' frameborder='0' scrolling='no' width='640' height='357' allowfullscreen></iframe>

Make your purchase and move on to the next step.

# Hosting: Where your files are going to live. 
Github pages it's my choice of hosting for static web pages because it is free and you can edit all your files inside of github without needing an editor. 

It's use is more oriented to programmers, but don't let this discourage you, once you get the hang out of it, it's going to be your (and your pocket) best friend.

For now create an account at [Github](https://github.com/), we are going to use it later.

<iframe src='https://gfycat.com/ifr/MellowAfraidAdamsstaghornedbeetle' frameborder='0' scrolling='no' width='640' height='382' allowfullscreen></iframe>

# The design
If you are a web designer you probably already have your webpage all set and ready to uploading, if you are like me, you will probably need to buy a theme or contract a designer to design your awesome page.

Unless, you take the time to search for free templates.

Here are some sites I go to search themes for my pages:
- [html5up](https://html5up.net/) free templates. (Be sure to checkout the [license](https://html5up.net/license))
- [themeforest](https://themeforest.net/category/site-templates/) templates for sale <$20 and give you support
- [templated](https://templated.co/) free templates

<iframe src='https://gfycat.com/ifr/ThoroughMenacingBasil' frameborder='0' scrolling='no' width='640' height='382' allowfullscreen></iframe>

Some of them are free others cost you less than $20.

If you choose a free template checkout the autors site and see if you can donate, they are giving away their hard work for you to use it freely, it is nice to reward them whenever you can. Also give credit where due.

# Stock Pictures: A powerful resource to make a normal website, beautiful  
Most modern web pages have those awesome pictures on the background, and they all have something in common: they are big, they are high-res and they are expensive... or not.

I have a list of sites where you can get free stock pictures with creative and commons license with free comercial use for anything you want.

- [unsplash](https://unsplash.com/)
- [pixabay](https://pixabay.com/)
- [pexels](https://www.pexels.com/) you can search here photos from other sites like unsplash and pixabay.

<iframe src='https://gfycat.com/ifr/HeavenlyAppropriateCopperhead' frameborder='0' scrolling='no' width='640' height='382' allowfullscreen></iframe>

Since you are getting them for free, I invite you to donate to the authors and communities for their hard work.

# SSL: The security aspect  

SSL (Secure Sockets Layer) is a standard technology to make an encrypted link between your server and the client, so all the information that is shared between the two of them is secure.

## Do I need a SSL Certificate?

3 reasons to have a SSL Certificate:

1. If you are getting data from users then you must have a SSL Certificate otherwise their data could be compromised.

2. Having a SSL Certificate improves your score on search engines, so your website can appear higher.

3. It builds trust on your visitors.

If you don't need anything from those reasons you can live without it.

Getting a SSL Certificate costs about $70 per year (like on godaddy), but there are other options.

Easiest one is to create an account at [cloudflare](https://www.cloudflare.com/plans/) and use the free service of one domain with ssl.

Harder is to use [letsencrypt.org](https://letsencrypt.org/) to generate your own certificate for free.

It is ok to use cloudflare for free when you have a small page and almost no traffic, but if you grow larger remind yourself to come back and start paying for the $20 plan that gives you added security and better performance.

If you choose letsencrypt.org I urge you to donate a bit to them, they are making a service which costs more than $50 yearly for free. They need the donations to continue to provide this service for free.  

We are going to configure the SSL Certificate later.

# Using your template to actually show your info  

I'll build a portfolio for myself to show you how to do it. 

Let's get our hands dirty.

Most templates files look the same, you see a bunch of folders and a bunch of files.
{% highlight shell %}
├── assets
│   ├── css
│   ├── fonts
│   ├── js
│   └── sass
├── elements.html
├── generic.html
├── images
│   ├── banner.jpg
│   ├── pic01.jpg
│   ├── pic02.jpg
│   ├── pic03.jpg
│   ├── pic04.jpg
│   ├── pic05.jpg
│   ├── pic06.jpg
│   ├── pic07.jpg
│   ├── pic08.jpg
│   ├── pic09.jpg
│   ├── pic10.jpg
│   └── pic11.jpg
├── index.html
├── landing.html
├── LICENSE.txt
└── README.txt

6 directories, 18 files
{% endhighlight %}

Let's find out what do you need to modify.

Open the index.html on your web browser.

<iframe src='https://gfycat.com/ifr/JointOrneryAllosaurus' frameborder='0' scrolling='no' width='640' height='357' allowfullscreen></iframe>

So that's the website, it still has the template text and titles, let's change that.

The title: Also known as the tab text.

I'm going to change it to Andre's Portfolio.
<iframe src='https://gfycat.com/ifr/PerfumedMealyGroundbeetle' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>

Next change the navigation title to your own.
<iframe src='https://gfycat.com/ifr/PinkFineHammerkop' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>

As you can see you can change the content of your page pretty easily, just search for the word(s) you want to change, modify it, save, and reload the page.

Change the
> Hi, my name is Forty
and the description below it, also remove the button.
<iframe src='https://gfycat.com/ifr/WarpedForsakenGossamerwingedbutterfly' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>

Keep doing this until you are satisfied with all the page. Remove anything you don't want.

So far we have this:
![webpage](/blog/images/editedWebPage.png)

Remember those stock photos I told you, now we are using them.
If you can recall from the directory structure, there were some images named like banner.jpg and pic01.jpg.
I'll make it easier, here:
{% highlight shell %}
├── assets
│   ├── css
│   ├── fonts
│   ├── js
│   └── sass
├── elements.html
├── generic.html
├── images
│   ├── banner.jpg
│   ├── pic01.jpg
│   ├── pic02.jpg
│   ├── pic03.jpg
│   ├── pic04.jpg
│   ├── pic05.jpg
│   ├── pic06.jpg
│   ├── pic07.jpg
│   ├── pic08.jpg
│   ├── pic09.jpg
│   ├── pic10.jpg
│   └── pic11.jpg
├── index.html
├── landing.html
├── LICENSE.txt
└── README.txt

6 directories, 18 files
{% endhighlight %}

Include your images to the same folder:
<iframe src='https://gfycat.com/ifr/LazyImpassionedBagworm' frameborder='0' scrolling='no' width='640' height='415' allowfullscreen></iframe>

Then you need to make the website show your images instead of the template images.

Things are turning technical, but follow me, this is the last step on before we mount the website.

There are two ways to show images: HTML or CSS. You need to search if the specific image you want to change is declared on the index.html or in css/main.css (normally you will have a main.css or base.css).

Search on the index.html for banner.jpg to see if it is declared there:
<iframe src='https://gfycat.com/ifr/MammothRightEsok' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>
... Nop, it is not there. 
Maybe in main.css
<iframe src='https://gfycat.com/ifr/MagnificentFrequentBrahmancow' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>
Oh, there it is. Change the name of the file to your file, in my case 'walking.jpg'.  
And reload the page.
<iframe src='https://gfycat.com/ifr/AmazingCreamyKarakul' frameborder='0' scrolling='no' width='640' height='386' allowfullscreen></iframe>
There, you made it.

Now add one more. 

Find pic01.jpg, looks like it is in index.html.

Change the name of the file to yours and refresh page.

<iframe src='https://gfycat.com/ifr/DifficultAssuredDikkops' frameborder='0' scrolling='no' width='640' height='369' allowfullscreen></iframe>

You can repeat this process for every image that you want to change.

If you only need, say 4 images, then delete the other images from the index.html file.

By now you should have all the abilities to modify your page, now it's time to...

# Mounting your site on Github pages  
Github is where you can version the code for your projects, basically it means that by uploading your code to Github gives you the ability to review every single change you or collaborators have done to your code. Which is awesome and will save you tons of time.

By itself Github won't run your code, that's why Github pages exists, you can host static websites on Github and show them on Github pages.

## Creating the project  
Open this link to [create a new repository](https://github.com/new).

For the repository name you must name it: [yourusername].github.io (In my case it would be: andregtz.github.io)

Otherwise it's not going to show up on github pages.

**Important: be sure to enable the 'Initialize this repository with a README' checkbox**. Otherwise it won't let you upload your files.

<iframe src='https://gfycat.com/ifr/SeparateLegitimateGemsbuck' frameborder='0' scrolling='no' width='640' height='370' allowfullscreen></iframe>

Here it doesn't let me name it like that because I already have that repository.

To have multiple pages you can name the repository 'otherpage' that will let you access your 'otherpage' with [username].github.io/otherpage.

My blog's repository name is blog and you can see it on [andregtz.github.io/blog](https://andregtz.github.io/blog).

## Uploading your content  

On your repository, click upload files button, select all the files of your site.
Wait until it uploads them.
<iframe src='https://gfycat.com/ifr/HilariousVainCat' frameborder='0' scrolling='no' width='640' height='368' allowfullscreen></iframe>

Now you should be able to see your content on: https://[yourusername].github.io/

If it doesn't appear go to settings and activate github pages.

<iframe src='https://gfycat.com/ifr/SoreSlimyGordonsetter' frameborder='0' scrolling='no' width='640' height='419' allowfullscreen></iframe>

If it still doesn't load try creating a file named '_config.yml' and putting your project name 
{% highlight yml %}
baseurl:/portfolio
{% endhighlight %}

<iframe src='https://gfycat.com/ifr/CommonBasicBaboon' frameborder='0' scrolling='no' width='640' height='419' allowfullscreen></iframe>

## Setting the domain name  

Go to godaddy.com.

On the top right corner click on your **profile name** -> **My Products**

![](/blog/images/godaddy-myProducts.png)

Click on **Manage** under **Domains**

![](/blog/images/godaddy-domains.png)

Under your site name click on the top right corner 'gear icon' and select Manage DNS.

It should take you to a page similar to this one:
![](/blog/images/godaddy-dnsManagement.png)

Search the add button, mine is on the bottom of the list. And click it.

You are going to add 3 new records for your domain.

1. Add a new record in type select: A, in host: @ and in Points to: 192.30.252.153 . Leave TTL as it is.
2. Add another new record in type select: A, in host: @ and in Points to: 192.30.252.154 . Leave TTL as it is.
3. Now add a new record but in type select: CNAME, in host: www, and in Points to: yourusername.github.io.

Mine looks like this:
![](/blog/images/records-1.png)
![](/blog/images/records-2.png)

You need to wait until the changes propagate over the network, it took less than 1 minute to me but it can take more time.

### Setting the domain name on Github

Go to your github repositorie and create a new document named CNAME, inside it write your domain name.
<iframe src='https://gfycat.com/ifr/PointlessImmediateAiredale' frameborder='0' scrolling='no' width='640' height='416' allowfullscreen></iframe>

Wait a couple of minutes to take effect and now you can enter your domain name in the browser and it should show you your page.
![](/blog/images/working.png)

## Setting the ssl  

Go to cloudflare.com and +add a Site, if your account is new it should take you directly to that.

![](/blog/images/cloudflare-addWebsite.png)
Enter your domain name. Click on Scan DNS Records. And wait about a minute. (When I did this it showed me that the scanning was done, but clicking on continue didn't do anything, just wait a couple of minutes more and try again. Took me about 5min)

Once the scanning is done click on continue.
![](/blog/images/scanning.png)
Verify that your records are listed, just verify that the registers that you added on godaddy are listed there. With this I mean de two A registers and the CNAME register.
![](/blog/images/verify-records.png)
Click on continue.

Choose the Free Website option.
![](/blog/images/free-website.png)

Click on continue.

Change the nameservers to the ones provided by cloudflare.
<iframe src='https://gfycat.com/ifr/UnknownGleefulGoat' frameborder='0' scrolling='no' width='640' height='446' allowfullscreen></iframe>

Check your email godaddy might ask you if you did this, confirm you did.

Next email you get should be from cloudflare saying that you have successfully added the website.

It can take 24hrs to see the change, once it finishes your webpage should say https before your domain name.

![](/blog/images/cloudflare-done.png)
![](/blog/images/https.png)


## Modifing your site inside Github  

By now everything was setup and you already have your website up and running.

The only reason you will need this part of the tutorial is when you want to change your website.

Fortunately Github lets you modify the files inside Github.

I'm going to modify my portfolio website and show you how I do it.

First I find the index.html of my project.

I click on edit.

Remember when you edited your index.html to show your information instead of the template text, well you are going to do the same here.

Search for the part that you want to change. In my case I want to change: "I'm a web developer" for "I'm a web & app developer, entrepreneur, computers systems engineer and technology enthusiast based in México."


Then I commit the changes and reload the page (notice that it takes a few seconds to update your changes on the site).

<iframe src='https://gfycat.com/ifr/NaiveImmediateIbisbill' frameborder='0' scrolling='no' width='640' height='460' allowfullscreen></iframe>

If you have more things to change repeat these steps for all the changes you want.


# Recap for the experienced

1. Get your domain name. If you already have one, continue.

2. Get a template either by searching it or by contracting a profesional designer.  
To look for templates look for sites like [html5up](https://html5up.net/), [themeforest](https://themeforest.net/category/site-templates/) and [templated](https://templated.co/).

3. Get your stock pictures to fill your site.
Some sites are [unsplash](https://unsplash.com/), [pixabay](https://pixabay.com/) and [pexels](https://www.pexels.com/).

4. Personalize your template and upload your code to github.

5. Redirect your domain name to your github pages project and create the CNAME file on Github.

6. Create a free account on Cloudflare and add your domain name, update your name servers on your Domain Name provider.

And that's it.

# Final notes

## Why I made this tutorial?  
I've noticed that there are a lot of people needing simple websites but don't have the resources to pay more than $200 yearly in a website that they still don't know if it's going to payback.  

This is my way to help out entrepreneurs and freelancers, I hope it helps.

## This is not the end...
If you already knew about these resources or better yet, you know more resources than I do then feel free to [fork this article](https://github.com/AndreGtz/blog/) and contribute to it. Maybe we can discover a budget way to get your apps online and compare with others the costs of our projects on each platform.

## About me
I'm 26yo currently, and I've been programming for 11 years. On my last year at college I discovered the entrepreneur culture and since then I read and try everything I get my hands on. This tutorial is part of one of my projects.

If you don't have time or feel stuck while building or migrating your website with my method then feel free to contact me and we can negotiate a price for my services.

## My Media
[Star me on Github](https://github.com/AndreGtz/)  
[Follow me on Twitter](https://twitter.com/blodvodhr)  
Send me a mail to <a href="mailto:andre@andrestefang.com" target="_top">andre@andrestefang.com</a>  
