---
title: Why is Google's encrypted dns controversial?
date: 2019-10-25
categories: privacy
permalink: /writing/why-is-googles-encrypted-dns-creating-controversy
---

The Wall Street Journal recently [broke the news](https://www.wsj.com/articles/google-draws-house-antitrust-scrutiny-of-internet-protocol-11569765637) that the House Judiciary Committee is investigating Google for a potential antitrust violation. There are concerns over Google’s plan to adopt encrypted DNS, a user privacy feature, in its Chrome web browser – a move that could, according to lobbyists, create a monopoly on acquired user data. Given the privacy violations across Silicon Valley in the past few years, it’s a little weird to hear that a new privacy feature could be anti-competitive. What’s really going on?

## What is encrypted DNS? Heck, what's DNS?

Encryption is the process of making data unreadable to anyone except the intended recipient. You use encryption every day, even if you don’t realize it:

- It makes your SnapChat pictures and iMessage conversations readable to only intended recipients
- It protects your credit card numbers when you shop online
- It keeps your neighbor from snooping on your Bluetooth phone calls
- It limits access to your home WiFi network to your friends and family

Domain Name Service, or DNS, is the system your network connected devices (phones, tablets, computers, smart appliances, etc.) use to turn names like [www.imarc.com](http://www.imarc.com/) into a series of dots and numbers that represent network addresses. 

DNS dates back to 1983, and like other internet protocols from that era, security wasn’t a design consideration. In 2019, DNS is one of the few pieces of the internet that hasn’t been wrapped in a layer of privacy-protecting encryption.

Each time you visit a website or use an app that accesses the internet – whether it’s Facebook, Fortnite, or FitBit – your device sends unprotected “clear text” requests for Internet addresses. Your ISP reads these – either directly via your ISP’s DNS servers, or indirectly via services such as Google’s [high-speed public 8.8.8.8 server](https://security.googleblog.com/2018/08/google-public-dns-turns-8888-years-old.html), CloudFlare’s [privacy-oriented 1.1.1.1 server](https://ppc.land/cloudflare-created-the-fastest-public-dns-beating-google-and-opendns/), or OpenDNS’s safety-oriented 208.67.222.222 server.

Encrypted DNS makes your device’s address requests private. This means your ISP can only see that you’re actively online, not what you’re doing. 

## For sale: Your personal data

The collection, buying, and selling of customer data without customer consent is entirely legal in the United States. In 2017, US Congress passed a bill making it [explicitly legal for your ISP to sell your browsing history](https://arstechnica.com/tech-policy/2017/03/for-sale-your-private-browsing-history/).

There’s a thriving economy around selling consumer data. Credit card issuers have sold consumer shopping histories for decades. Among various purchases and trends, there’s a remarkable level of detail available. Did you know there’s a distinct credit charge code for massage parlors (7297), alimony and child support payments (9211), or bail/bond payments (9223)? MasterCard and American Express create about $400M in revenue each year selling this kind of data.

In the past decade, the consumer data economy has exploded in size. As a Forrester analyst [said in 2013](https://adage.com/article/dataworks/mastercard-amex-feed-data-marketers/240800), “Anybody that's got data right now is in the business of trying to make money off of it.”

Internet Service Providers (ISPs) like Comcast, Verizon, or AT&T are responsible for a significant portion of these data sources. Using techniques such as [deep packet inspection](https://digitalguardian.com/blog/what-deep-packet-inspection-how-it-works-use-cases-dpi-and-more), ISPs are able to monitor website visits and sell visitors’ behavior data.

If you think your ISP won’t sell that data, let me direct you to some proof that they’re [selling your precise location](https://arstechnica.com/tech-policy/2019/01/t-mobile-sprint-and-att-still-selling-your-location-data-report-says/) to anyone willing to pay. On the fixed-network side, Comcast, Verizon, and AT&T [vigorously fought a California bill](https://arstechnica.com/tech-policy/2017/09/isps-claim-a-privacy-law-would-weaken-online-security-and-increase-pop-ups/) that would have required permission from customers to sell their data. For years, providers have served targeted ads to their customers based on this collected data. 

## So what is Google doing?

Google is the developer for the immensely popular Chrome browser. While Google has come under some well-deserved scrutiny for privacy issues, the Chrome development team does seem to genuinely care about user privacy. They’ve been working to add DNS-over-HTTPS (DOH) support to the Chrome browser since 2016, with an expected rollout later this year.

ISPs have created a lucrative side business from being able to snoop on their customers’ traffic. The major shift towards [using HTTPS protocol](https://www.imarc.com/blog/the-https-train-leaves-the-station) in recent years has put a dent in ISPs’ ability to sell data. DOH could be the final nail in the coffin for that revenue stream. 

Google’s Chrome is the main web browser on 64% of PCs and over 80% of mobile devices. If Chrome switches everyone over to encrypted, private DNS, there goes two-thirds of that revenue. Not only that, Mozilla announced it’s rolling out its own [DOH encryption for the Firefox browser](https://blog.mozilla.org/futurereleases/2019/09/06/whats-next-in-making-dns-over-https-the-default/). 

## Who else supports Encrypted DNS?

So far, it’s a short list: [Mozilla's Firefox](https://support.mozilla.org/en-US/kb/firefox-dns-over-https) and [CloudFlare](https://developers.cloudflare.com/1.1.1.1/dns-over-https/).

Mozilla has been working with CloudFlare to [add DNS privacy to Firefox](https://hacks.mozilla.org/2018/05/a-cartoon-intro-to-dns-over-https/). As a distant fourth place in the web browser market, Firefox doesn’t threaten ISPs the way Chrome does, so it’s largely gone unnoticed by ISPs.

Thus far Apple and Microsoft have been silent on DNS privacy. Apple’s Safari engineers have focused on [aggressive “Intelligent Tracking Prevention”](https://webkit.org/blog/category/privacy/) features, but haven’t really looked into the network layer like the Chrome team has. While Microsoft’s Edge browser was not designed with privacy in mind, developers did [start testing](https://blogs.windows.com/msedgedev/2019/06/27/tracking-prevention-microsoft-edge-preview/) a tracking prevention feature earlier this summer. DNS does not appear to be on their radar.

## Lobbyists swing into action

With Google threatening to cut off a comfortable revenue stream, the cable and telecom industries’ lobbying initiatives have picked up. NCTA, CTIA and US Telecom sent a [joint letter](https://www.ncta.com/sites/default/files/2019-09/Final%20DOH%20LETTER%209-19-19.pdf) to the House Judiciary Committee. It started quite reasonably…

> By interposing itself between DNS providers and the users of the Chrome browser (> 60% worldwide share) and Android phones (> 80% worldwide share of mobile operating systems), Google would acquire greater control over user data across networks and devices around the world. This could inhibit competitors and possibly foreclose competition in advertising and other industries.

But they promptly jumped the shark, claiming:

> Moreover, the centralized control of encrypted DNS threatens to harm consumers by interfering with a wide range of services provided by ISPs (both enterprise and public-facing) and others. 

The letter cited everything from network management to protecting children from pornography to back the anti-trust claims being made. Nowhere does the letter mention that selling customer data is a revenue source that is in jeopardy.

## The fight over encrypted DNS is about money

When somebody threatens an established industry’s revenue, of course there will be a fight. The controversy, in this case, is a result of one side using Congress as leverage against the other. There is a case to be made that Google could use encrypted DNS to lay claim to more customer data and lock out competitors, but the issue is being heavily blown out of proportion by ISPs.

Encrypted DNS is not an anti-competitive technology. It improves customer privacy in an environment where unprotected data is farmed and distributed for profit. In an ideal world, privacy with strong encryption should be an invisible part of any digital data system. Google is pushing the technology forward by adding it to the Chrome browser. Many of us are hopeful that this will spur the rest of the industry to get on board.

Privacy shouldn’t be a controversy.\
**Privacy is a human right.**


## Further Reading:

- Technology
	- [A Cartoon Intro to DNS over HTTPS](https://hacks.mozilla.org/2018/05/a-cartoon-intro-to-dns-over-https/) - Mozilla
	- [How to Keep Your ISP's Nose Out of Your Browser History with Encrypted DNS](https://arstechnica.com/information-technology/2018/04/how-to-keep-your-isps-nose-out-of-your-browser-history-with-encrypted-dns/) - Ars Technica
	- [Mozilla to Gradually Enable DNS Over HTTPS for Firefox US Users Later This Month](https://www.zdnet.com/article/mozilla-to-gradually-enable-dns-over-https-for-firefox-us-users-later-this-month/) - Zdnet
	- [DNS Security](https://ns1.com/dns-security) - NS1
	- [DNS Over HTTPS Guide](https://cleanbrowsing.org/guides/dnsoverhttps) - Cleanbrowsing.org
- Technology - Deep into the Weeds
	- [DNS Over HTTPS](https://www.chromium.org/developers/dns-over-https) - Chromium Developers
	- [DNS Queries over HTTPS (DoH) - 2018 Public Release Draft, P. Hoffman (ICANN) & P. McManus (Mozilla)](https://tools.ietf.org/html/draft-ietf-doh-dns-over-https-14)
	- [Pros and Cons of DNS Over HTTPS](https://www.netsparker.com/blog/web-security/pros-cons-dns-over-https/) - Netsparker
- News and Policy
	- [Mastercard, AmEx And Envestnet Profit From $400M Business Of Selling Transaction Data](https://www.forbes.com/sites/petercohan/2018/07/22/mastercard-amex-and-envestnet-profit-from-400m-business-of-selling-transaction-data/#7c5e97497722) - Forbes
	- [Google Now Tracks Your Credit Card Purchases and Connects Them to Its Online Profile of You](https://www.technologyreview.com/s/607938/google-now-tracks-your-credit-card-purchases-and-connects-them-to-its-online-profile-of-you/) - Technology Review
	- [House Antitrust Investigator Now Scrutinizing Google's Plans to Add DNS Encryption to Chrome](https://gizmodo.com/house-antitrust-investigators-now-scrutinizing-googles-1838601830) - Gizmodo
	- [Why big ISPs aren’t happy about Google’s plans for encrypted DNS](https://arstechnica.com/tech-policy/2019/09/isps-worry-a-new-chrome-feature-will-stop-them-from-spying-on-you/) - Ars Technica﻿

*This post originally published at [www.imarc.com/blog/why-is-googles-encrypted-dns-creating-controversy](https://www.imarc.com/blog/why-is-googles-encrypted-dns-creating-controversy)*