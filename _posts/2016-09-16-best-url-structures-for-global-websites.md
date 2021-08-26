---
title: Best URL structures for global websites
date: 2016-09-16
categories: seo
permalink: /writing/best-url-structures-for-global-websites
---

*This post co-written by Robert Mohns and [Dave Tufts](https://www.imarc.com/about/dave-tufts).*

When working on a multi-lingual or regionalized website, one of the first and most important decisions is how to handle URLs. Do you use ccTDLs? Country-codes subfolders? Subdomains? Do you want `mysite.co.uk` or `mysite.com/uk` or `uk.mysite.com`?

These decisions have a tremendous impact on your SEO, how people perceive your brand as a whole, how local search engines view your brand, as well as the internal politics of each region or division within your brand.

Before we start jet setting around the globe, let’s review some terminology.

## Terminology

- **ccTLD** stands for Country Code Top Level Domain. This is the last part of a domain name that contain a country code – `.co.uk` or `.fr` instead of `.com` or `.org`. (Trivia: the ccTLD system was created in 1984, when the early Internet was still called ARPA-Internet.)
- **gTLD** stands for Generic Top-Level Domain. They have no designated geographic affinity. Examples are `.com`, `.info`, `.gov`, and `.com`. (But note that .com connotes a US site. More on that later.)
- **Country-coded folders** is when all content lives on the same domain but is segregated within a folder: `mysite.com/uk/mypage.html`
- **Domain Authority** is a score that predicts how well a website will rank on search engines based on inbound links, number of total links, age of domain, trust, etc.
- **Geo-targeting boost** related to SEO refers to how search engines can automatically recognize ccTLD content and give preference based upon the searcher’s location. For example, search engines typically only show ccTLD results if the search is performed on the localized version of the search engine. So a search on `google.co.uk` will return results from `.co.uk` as well as `.com`, `.net`, `.org` and any other non-localized top level domain. But `google.co.uk` will probably not promote results from `.fr`, `.nl`, or other ccTLD domains. Google also provides the Webmaster Tools Search Console to configure sites for geo-targeting that do not use ccTLD.
- **PageRank** is Google’s measure of any given web page’s importance among all known web pages. Higher is better, but it is only one of at least 200 other factors used to rank a page.


## Folders vs Subdomains vs ccTLD in International Seo

Let’s start with some example URLs:

- `mysite.com/uk` is a country-coded folder.
- `uk.mysite.com` is a sub-domain
- `mysite.co.uk` is a ccTLD

What are the SEO and usability pros and cons for each?

### Country-coded folders on an existing site

Every site is unique, but using country-coded folders is usually our recommendation, or at least our starting point. It has a lot of advantages:

- Makes use of existing strong domain authority
- Strengthens domain authority over time
- Minimizes maintenance costs over time
- All content is easily managed in a single place
- Google Analytics (and similar tools) can be consolidated with no extra work
- Integration points are streamlined through a single domain

You can geo-target these folders using [Google Search Console](http://www.google.com/webmasters/tools/home?hl=en). (You can do this for Bing and Yahoo searches using the [Bing Webmaster Dashboard](https://www.bing.com/webmaster/help/geo-targeting-your-website-b7629197).) While not as automatic and effective as ccTLDs, configuring this is just a simple form in Google’s and Bing’s webmaster tools.

**Potential downsides:** May not perform as well in country-specific search engines (such as google.co.uk or yandex.ru), and might confuse users that expect a ccTLD.

### Subdomain of an existing site

Subdomains help users understand that they are looking at a local version of a global site they may be familiar with. And, it makes it possible to host each site in the country it serves, which provides a modest geographic SEO bonus.

As with folders, you can geo-target subdomains.

**Potential downsides:** Many visitors type `www.` for any website, so they may not ever see the correct subdomain. And while it used to be true that you could get an SEO bonus based on your parent domain (`mysite.com`), it’s not anymore. The subdomain technique was so heavily abused that Google and Bing no longer assign much inherited domain authority to that relationship.

### ccTLD as a separate site

ccTLDs have an automatic and highly effective geo-target bonus, they are very intuitive for users, and like subdomains you can host the site in its local country. They tend to perform well in local search engines (such as google.co.uk or yandex.ru), when the search term is obviously local.

**Potential downsides:** Expensive to maintain, as many CMS systems don’t gracefully manage separate TLD sites and securing a local domain can be difficult for a foreign company. New ccTLD sites don’t get any SEO bonus from pre-existing sites.


## Comparison in pictures

Moz, one of the authorities on inbound marketing and SEO, prepared these charts showing the relative impact of different approaches:

![](pros-cons-cctdlvs.png)\
![](cctdls-moz.png)

If you are measuring PageRank, it’s worth nothing that these approaches are all PageRank-neutral. Inherited domain authority and geo-targeting are more influential.


## Perceptions Matter

The `.com` top level domain is derived from "commercial”. That sounds neutral, but in actuality it is viewed as US-centric around the globe. Other countries have their own commercial equivalents such as `.co.uk` (UK) or `.com.mx` (Mexico) or `.co.jp` (Japan). And, although to a lesser degree, `.org` and `.net` are also associated with the United States.

Users prefer to browse locally. They are aware of TLDs and make some decisions based on ccTLD, especially when looking to purchase something locally. Your pre-existing brand influences the click, of course, and ultimately content plays a deciding role after they actually arrive at your site.

The search engines have their own ideas too. Using a country code top-level domain strongly implies your website is meant for a specific country or region (e.g., .de = Germany, .eu = Europe).

[Generic Top-Level Domain (gTLD) Vs. Country Code Top-Level Domain (ccTLD)](http://www.tricksbag.com/gtld-vs-cctld/) discusses the SEO benefits of ccTLDs:

> Search engines also take that in consideration while ranking your website in different regions. Just see the difference for instance:
> - `https://www.google.com/search?q=pizza+shops`
> - `https://www.google.co.in/search?q=pizza+shop`
> - `shttps://www.google.co.uk/search?q=pizza+shops`
> - `https://www.google.com.au/search?q=pizza+shops`

You will find that most of the websites ranked in each version are with that particular country’s ccTLD. You will find very few websites with .com, .net etc.

This does not apply so much to multi-national brands. Google understands that a search for a “pizza shop” is a very local search, but searching Google’s UK site for “digital banking solutions” returns almost all .com results on the first page: [www.google.co.uk/#q=digital+banking+solutions](https://www.google.co.uk/#q=digital+banking+solutions)

Also, are you sure that you should be localizing your site? Pizza slices may only be relevant within a few miles (well, [usually](https://www.google.com/#q=pizza+on+the+ISS)), but [pizza peels](https://www.google.com/#q=pizza+peel) can be shipped anywhere, and [pizza-making advice](https://www.google.com/#q=pizza+making+advice) is universal. Don’t limit yourself unnecessarily.


## What does Google say?

Google’s algorithm is secret, but because they want great content to succeed they provide a lot of guidance. Google Webmaster Central’s [Internationalisation FAQ](https://sites.google.com/site/webmasterhelpforum/en/faq-internationalisation) has this to say about URL structures:

> It helps to have the country-specific sections of the site clearly separated on a per-country basis. You can do that either by using ccTLDs or by correctly configuring gTLDs in Search Console. With gTLDs you can use subdomains (`country.example.com/`) or subdirectories (`example.com/country/`); either way is fine.

In other words, **Google really doesn’t care** which of these approaches you use, so long as it’s clear and obvious to visitors.

(Meta tags can and should be used to indicate a document’s language, but Google does not use them for geotargeting.)

## Trends

A number of international brands seem to be moving away from ccTLDs to a single domain. It tells the world that it’s one company, one brand, with international reach. Even if your business is traditionally local, a single domain may still be the right move.

Even the British staple *The Guardian* moved away from ccTLDs to subfolders:

- `www.theguardian.com/uk`
- `www.theguardian.com/us`

The Guardian wrote extensively about their migration away from ccTLDs here:

- [theguardian.com is our new domain, as of today](http://www.theguardian.com/help/insideguardian/2013/jul/30/the-guardian-dot-com)
- [How the Guardian successfully moved domain to www.theguardian.com](http://www.theguardian.com/info/developer-blog/2014/feb/18/how-the-guardian-successfully-moved-domain)
- 
We can’t overlook the long-term benefits of ease of maintenance and increased domain authority of a single domain, especially when your offerings aren’t heavily local.


## Conclusion

You want to employ a solution that is overall best for **SEO, brand presentation, and return on investment** for years to come. You don’t want any geography’s users to feel like second-class visitors, nor do you want to waste resources on barely-used sites.

Several Imarc clients, including Datalliance, Bottomline Technologies and Fourth, have adopted the subfolder approach as the best solution for them. But as they say in advertising, “Your mileage may vary”.

* * *

## Further Reading

Moz is one of the authorities on SEO. We suggest starting with [What are ccTLDs?](https://moz.com/learn/seo/cctlds) and [International SEO](https://moz.com/learn/seo/international-seo).

Jesper Jørgensen wrote an excellent deep dive on the pros and cons of the three main localization structures for Moz: [Folders vs Subdomains vs ccTLD in International SEO - An Overview](https://moz.com/ugc/folders-vs-subdomains-vs-cctld-in-international-seo-an-overview). Jørgensen also provides a break-even calculator to help you decide whether a ccTLD is worth the initial investment.

To understand how ccTLDs are perceived by international visitors, dig into [How Searchers Perceive Country Code Top-Level Domains](https://moz.com/blog/cc-tld-domain-study). This study is a fantastic collaboration between Moz and Hubspot.

Google’s Webmaster Central blog has a useful [Internationalision FAQ](https://sites.google.com/site/webmasterhelpforum/en/faq-internationalisation). If you love digging into the nitty-gritty of implementation, this page is for you.

* * *

*This post was originally written for and published at [www.imarc.com/blog/url-structures-for-global-websites-and-seo](https://www.imarc.com/blog/url-structures-for-global-websites-and-seo)*