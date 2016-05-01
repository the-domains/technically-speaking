---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
keywords: []
description: 'My girlfriend had been enamoured. 300 hundred plus code enthusiasts, students and professionals all working together. It encompasses all that she loves about technology. Projects to change the world, forging bonds and harnessing ideas or just there to learn a new language or framework.'
datePublished: '2016-05-01T12:05:23.954Z'
dateModified: '2016-05-01T12:05:05.582Z'
title: //HackZurich
author: []
authors: []
publisher:
  name: null
  domain: null
  url: null
  favicon: null
starred: true
sourcePath: _posts/2016-05-01-hackzurich.md
published: true
url: hackzurich/index.html
_type: Article

---
# //HackZurich

My girlfriend had been enamoured. 300 hundred plus code enthusiasts, students and professionals all working together. It encompasses all that she loves about technology. Projects to change the world, forging bonds and harnessing ideas or just there to learn a new language or framework.

That was back in _2014_, and I wish I'd joined her then. I had a horrible feeling **I wouldn't be up to much, **and that I was lacking the talent and knowledge to contribute. Attending the [Game Jam in 2015 ][0]taught me that this isn't the point... you bring your own unique talents by turning up, and you learn a huge amount by just mucking in and getting things done. And the whole thing is about learning, not showing off.

So one year on, and one hackathon behind me, it was time for a bigger event. One that I was scarcely prepared for.
![](https://s3-us-west-2.amazonaws.com/the-grid-img/p/17af9ad6a6a326cc37bf408f3ff5f5bfdef1e05b.png)

## [http://hackzurich.com/ ][1]

## Swag

On arrival, everyone wants to be your friend. Well, the organisers and sponsors do at least. And to be fair, they're generous throughout the whole event with their time, guidance and support. From Swisscom embossing a pillow with your name in celebration of their "cloud", to bundles of sun glasses and back packs...
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/8aba0847-0fdf-46d9-bb2c-5ff86150b7f0.jpg)

There were more relevant gifts and promotions too in the form of free service usage for the cloud or a cool api.

Some companies handle it better than others... Seeing the head of Samsung take to the stage and bad mouth small companies was a little odd. But on the whole It works well, offering you the chance to step out of your shoes and try something new. ![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/ec082c3c-e28b-4ab1-b699-c7fe3cb58f52.png)

## Tech Selection

So after the companies have had a chance to present their technologies on stage, at their booths or through their swag, people turn their minds wholeheartedlyto what they want to make. Some have firm ideas already before arriving and arrive as teams. My partner and I wanted to work together, but other than that...

* _We knew we wanted a web project & to try some cloud hosting._

* _We knew we wanted to help people in need, not just make a dollar_

This wasn't really a clear enough remit for a speech to others in our position (around 200 people), so we went into "clearing" at around 11 PM and watched people with ideas but no team give a speech. Chris was the presenter that caught our eye, with his clearly passionate attitude - wanting to do something to help people in need. Then we met Nicco who joined to make a team of four. Enthusiastic and full of energy, he was keen to learn and help.

**So what was the plan?**

We were wanting to use the 1000s of Kiosks in Switzerland and Europe to connect existing consumers with strangers in need, and help make their day a little better.

When buying your goods, you'd have the option to buy a coffee, gipfeli (a Swiss croissant) or something else from a list of products, that could be received by a stranger. 

Obviously, the trust element wouldn't be to everyone's taste, as someone could take advantage of the system. But we wanted to trust in the community. And we like the idea that a student, busy parent or anyone down on their luck could benefit, as well as people in more long term difficulty.

Of course, it's still powered by the conventional consumerist nature, with a sale being generated for the Kiosk with each charitable action... But we need to demonstrate a benefit to the companies involved to make use of their infrastructure.

And so... _Karma Coffee_ was born

We fell into our roles reasonably dynamically, and selected technologies around 1am:

* Cloud instance of flask as a web server to communicate with (hosted on Azure)

* Backend api from the Kiosk system (run by 3rd party promotion tracker)

* Customer portal website (Nicco's project in angular.js & HTML5)

* Back end interface (Running at the checkout, and able to handle tokens for gifts)
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/c1653300-1185-4aec-911a-3d9cf6a3aabd.png)

## Knuckle Down

With the technologies needed defined and the first night setting in, it was time to start work in earnest. With our own areas to work on and a good idea of what we wanted to achieve, it started out with good optimism considering the sleepless work we were prepared for.

And then the problems started.

Its worth stressing that nothing was beyond our grasp. But its surprising how the tired mind can become so inefficient... 

* Flask was / was not available in the in-between state of the MS platform, depending on how you tried to setup your project.
  * _Using AWS and the Swisscom alternatives weren't helping._
* The interface to the loyalty platform used an archaic form of SOAP communication.
  * _My girlfriend had to develop a way to interrogate the service as the documentation was wrong_
* We found that the system held only dummy data. 4 entries without any interesting or useful data...

The following morning the Kiosk team helped us out with credentials & explained they couldn't provide real data. So... we enriched it. We added in actual locations of stores, addresses and a bunch of details that would be accepted by the SOAP messaging system.

Flask was more of an issue still, as we needed to get it to interact with the API. Running it locally wouldn't be enough of a real world test. Eventually, we scrapped this, and made the service run on a local instance and broadcast to the web aps using our own security. 

With a good nights sleep, it only took an hour or so for 2 of the team to independently identify the issue. But these are the kinds of problems you can expect from working in a sleep deprived team.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/849eb6f7-b438-458f-8854-55ebe6f7fa6d.jpg)

> Stepping out into the cold days, and colder nights... time was passing with little or no meaning to us.

I remember a dub step playing violinist at one point in the evening of the 2nd night, but the whole thing seems surreal. Fortunately, we were fed a variety of foods regularly to keep us nourished at least. By stages, we started to arrive at a working product, and prepared ourselves for a presentation to a small board of judges to show off our working model, and the concept behind it. 

## Finale

With my partner having been a finalist (top 20 team), her hopes were for a repeat of 2014\.

> In the 2014 //Hackzurich : she was doing sentiment analysis for conflict zones, searching for commonality in digital activity between warring nations.

Though we may have been a little disappointed, we were proud of what we accomplished. A working model of what had only been an idea less than two days ago, and demonstrable (with a lot of effort) in front of a panel of judges, away from our workstations and using the internet. We had a congratulatory get together in Frau Geralt's Garten, enjoying a few rays of sunshine together.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/40cc19c9-7841-4227-8998-59147df300b8.jpg)

And then the closing speeches and presentations were also a pleasant way to round out a crazy 48 horus.

I remember feeling encouraged and discouraged by overhearing a comment, that it was the kind of project we'd carry on working with, without encouragement from the Kiosk team. I believe it was a bingo app that won their recommendation in the end, and there's was certainly more fully featured and production like than ours. It's an important reminder though, at the end of the day, the sponsors are happy to help you as long as their agenda is being met. What you get as a contributor get out of the event needs to be in the days that follow those 48 hours, and what they inspire you to create or who to become.

Looking back on that time -- even though its only months rather than years -- I feel the inspiration that was instilled to do more is the greatest take away. The learning experience is an additional bonus, and will be different for every attendee, but we can all try and lift each other higher, and help achieve something today, and for the future.

[0]: null
[1]: http://hackzurich.com/