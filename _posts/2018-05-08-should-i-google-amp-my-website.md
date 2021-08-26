---
title: Should I Google AMP my website?
date: 2018-05-08
categories: seo
permalink: /writing/should-i-google-amp-my-website
---

This spring I’ve been getting a lot of questions about Google AMP and what it means for my clients’ websites. AMP, or Accelerated Mobile Pages, is a framework for creating hyper-mobile-friendly pages. Announced by Google in late 2015, AMP pages began appearing in search results last spring.

In this article, I’ll discuss what AMP is, some pros and cons of adding AMP to your website, who benefits from AMP, and whether you should AMP your site.

* * *

## What is Google AMP?

Created by Google as a semi-open response to Facebook “Instant Articles” and Apple News (more on that below), AMP is a kind of web page that strips out nearly everything but the content to make pages load really, really fast. 

AMP pages load in the blink of an eye. Literally. Even on slower phone networks. This is *fantastic* for mobile users, especially given that the trend to responsive web design has lead to pages which are paradoxically well-designed for mobile yet slow to load. (BostonGlobe.com, I’m looking at you.)

Any website can publish AMP pages. Which leads to the obvious question: Should you AMP your site?

## Why add Google AMP to my site?

First, of course, it provides a great user experience for your visitors. Second, due to its underlying technical model, it neatly circumvents content blockers that stop ads from appearing. Third — and let’s be honest, this is the big one — **Google will give your AMP pages special treatment**.

Google shows AMP results *before all other search results*. If you have an AMP page, and it is relevant to the search, you probably go into a carousel of promoted content, at the top of the search results. *I can’t emphasize enough what an advantage this is.*

![](/images/blog/amp-example-serp.png) ![](/images/blog/amp-example-serp-2.png)

Google officially says that AMP is just one of many signals for rankings. That’s true. There are a lot of signals, including whether a page is mobile friendly (c.f. [Mobilegeddon](https://www.imarc.com/blog/life_after_mobilegeddon)) and fast. AMP is those in spades.

I’ve been asked if Google is unfairly favoring AMP pages with this scheme. It depends on how you interpret the rules. AMP alone won’t get your pages higher in the rankings than would a nice, fast mobile-friendly site. But if you rank at all, you get promoted above traditional search results.

Fair? Unfair? I’ll leave that to you.


## Why not add Google AMP to my site?

Aside from the extra effort required to add an AMP site to your main site, of course? The most compelling reason is that AMP web addresses don’t live on publishers’ sites, but at Google.com.

As Google [recently described](https://developers.googleblog.com/2017/02/whats-in-amp-url.html), there are three web addresses involved in an AMP page:

- **The original URL on your site:** [http://www.imarc.com/amp/blog/...](http://www.imarc.com/amp/blog/thisblogentry.html)
- **AMP cache URL**, which most users never see and we can ignore.
- **The Google AMP viewer URL:** This is what appears in your phone’s web address bar: [www.google.com/amp/www.imarc.c...](http://www.google.com/amp/www.imarc.com/amp.blog/thisblogentry.html) means that anyone that shares your AMP page isn’t sharing your website, so your site doesn’t get an SEO boost from it. The algorithmic underpinnings of modern web search is that publicly available links are votes for relevancy (this is true regardless of whether the engine is Google, Bing, Yandex or Baidu). No links = no votes = no PageRank contribution.

There are other issues. Branding is limited; AMP sites look like Google sites rather than their own brand. Video, social media posts, advertising, animations, audio and analytics can be delivered only using Google’s AMP components. All JavaScripts must be one of the pre-approved Google scripts hosted on the Google AMP content delivery network. 

![Who owns this URL? Not Forbes.](/images/blog/amp-example-article.png)\
*Who owns this URL? Not Forbes.*

All said and done, when you use AMP you are locking yourself into Google’s tools, rather than the open standards that underpin the rest of the Internet.

## Why does AMP exist?

Google’s mission is “to organize the world's information and make it universally accessible and useful”. In doing this, it has become the world’s most profitable advertising agency, and works tirelessly to stay at the top.

Facebook’s “Instant Articles” format and Apple’s News format pose a challenge to this hegemony. If Facebook and Apple can get people to read more of the web inside Facebook and Apple News, they can siphon advertising revenue from Google, while also undermining Google’s status as the Internet’s de facto start menu.

Both Apple News and Facebook Instant Articles are locked to their respective platform owners. For content creators, this is a bit of a Faustian bargain. But, at least web site owners control their own URLs with these systems.

Google AMP is a pitch to provide an open alternative. But, since the canonical URLs are controlled by Google, the advertising is controlled by Google, the analytics model is controlled by Google, and the entire interactive element is controlled by Google, it’s no less a Faustian bargain for publishers. Just a different one.

![Google is the Start Button of the Internet](start-button-of-the-internet.png)


## What kinds of sites should have AMP?

By now you’re thinking *"Just tell me if I should use it!"* Sorry, the jury is still out.

**News publishers should try AMP.** Most have seen higher click-through rates into their sites for all Google, Facebook and Apple’s offerings — although not all have seen that turn into more advertising revenue. Some of the big ones, such as The Guardian, have dropped Facebook and Apple; I haven’t yet heard of anyone dropping AMP. 

The Guardian reports that 60% of Google-referred mobile traffic comes via AMP, and click-through to non-AMP pages is 8.6% higher than from their regular mobile pages. That’s enough a gain to take seriously.

**Commerce sites** with AMP haven’t yet shared much data. One marketer shared AMP commerce results, seeing an uplift in traffic but a fall in engagement, and more orders but lower average order value. Saying that’s “odd” is an understatement of British proportion. The Magic 8 Ball says: Outlook unclear.

> *UPDATE: A friend provided a plausible explanation for this; see end of article.*

**B2B and lead generation sites may benefit.** AMP pages do get more visits from search and can get more conversions, but it’s not clear if they are of the same quality or not (c.f. the commerce oddness above). It is worth a try, but if you already provide a fast and clean mobile experience to your visitors, your development hours are probably best spent elsewhere. (Use [Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) to see how fast and friendly your mobile site is.)

In all of the above cases, if your direct competitors are using AMP already, you should too. And if they aren’t, you should seriously consider it. (Which is why you’re reading this, right?)

## Why not just a fast mobile site?

Why, indeed. Google already favors fast, mobile-friendly sites in its search results. The main reason to adopt AMP is to get that special treatment from Google.

After a year with amp, it looks like Google AMP is a lot like Facebook Instant Articles and Apple News: it benefits its creator more than it benefits website owners. Which is to say, you.

Ultimately, I’m not convinced that AMP is in the long-term best interest of the web. I admire AMP’s focus on great user experience and extreme performance, but in terms of return on investment, it’s the new “m-dot” dedicated mobile website — worth it for specific scenarios, but not the best approach for everyone. 

![Blackberry phone with Google on-screen](/images/blog/blackberry-mobile-internet.png)\n
*It’s great for some situations. I guess.*

## Update: A plausible explanation for the commerce effect noted above

An old friend of mine sent me this observation:

> …The uplift in traffic but drop in engagement doesn't seem odd at all. We know that there are differences in user engagement depending on if they access content while stationary or mobile, on which browser the user uses, on the demographics of the user and on how the user reaches the site. […] If the incremental traffic is from users who are on the move, using a client that defaults to Google for search and going to the site as a result of click on a promoted search result is it really a surprise that the engagement is lower? Furthermore, Android users are probably more likely to find things through Google and statistically Android users spend less, which could well account for the drop in order value.

I am not totally convinced but it's quite plausible. And even if order value is lower, an incremental increase in revenue would still be welcome to any retailer, presuming that business is profitable.

As always, "your mileage may vary." If you run a commerce site, I encourage you to give AMP a try.

* * *


## Further Reading

- Business AMP Topics
[	- Are Google Accelerated Mobile Pages (AMP) Worth Marketers’ Time?](http://www.seerinteractive.com/blog/google-accelerated-mobile-pages-amp-worth-marketers-time/) - Seer Interative
	- [AMP Implementation and Google Rankings – Is it Really Worth Doing?](https://bynd.com/news-ideas/amp-implementation-and-google-rankings-is-it-really-worth-doing/) - Beyond
	- [Google AMP Gets Mixed Reviews From Publishers](https://www.wsj.com/articles/google-amp-gets-mixed-reviews-from-publishers-1477648838) - Wall Street Journal (paywall)
	- [Some Publishers Cool on Google AMP](https://www.nytimes.com/2017/01/01/technology/google-amp-mobile-publishing.html) - New York Times
	- [The Guardian pulls out of Facebook’s Instant Articles and Apple News](http://digiday.com/media/guardian-pulls-facebooks-instant-articles-apple-news/) - Digiday
- Technical AMP Topics
	- [What’s in an AMP URL?](https://developers.googleblog.com/2017/02/whats-in-amp-url.html) - Google Developers Blog
	- [Is Google AMP Worth It? Three Real-World Case Studies](http://www.stateofdigital.com/google-amp-case-studies/) - State of Digital
	- [Implementing Accelerated Mobile Pages (AMP)](https://www.tunetheweb.com/blog/implementing-accelerated-mobile-pages/) - TuneTheWeb.com
	- [The Problem with AMP](https://80x24.net/post/the-problem-with-amp/) - Code vs. The World

*This blog was originally written for and published on [www.imarc.com/blog/should-i-google-amp-my-website](https://www.imarc.com/blog/should-i-google-amp-my-website)*