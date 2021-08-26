---
title: How is a CMS like a coffee maker?
date: 2019-04-18
categories: seo
permalink: /writing/do-sites-really-need-a-sitemapxml-for-good-seo
---

It's taken as [received wisdom](https://en.wikipedia.org/wiki/Received_wisdom) that good SEO requires a [sitemap.xml file](https://support.google.com/webmasters/answer/156184?hl=en). This is so well established that every “SEO audit" tool checks for the existence of a sitemap.xml file and complains bitterly if it's not there. There is no shortage of SEOs saying a sitemap.xml is practically mandatory. But does SEO really benefit from a sitemap file?

WHAT PROBLEM DOES SITEMAP.XML SOLVE?

Google created the sitemap.xml in 2005 to fix a problem – it exposed content that the search engines could not find otherwise.

This was a big deal – that was still in the era of sites which heavily used Flash, Silverlight, Java, and JavaScript for navigation and content. These practices were [starting to change](https://alistapart.com/article/dropdowns), but it was a slow process.

Content that can’t be found by clicking around on a website is a problem sitemaps help to solve. To a human it is trivial to type what they’re looking for into a search field and press “Submit”. To a machine, that's complex. Humans can infer from context and are thinking about what they want; machines require definite instructions.

Sitemaps also allow very large websites with poor internal linking to make sure that content is found by search spiders.

But… A few things have changed in the 14 years since the creation of the sitemap:

- Google can run and read JavaScript
- Google can run and read Flash (besides which, Flash is walking dead: [Even Adobe has finally given up](https://www.wired.com/story/adobe-finally-kills-flash-dead/) on the security dumpster fire known as Flash Player)
- Silverlight [is dead](https://www.theregister.co.uk/2015/07/02/microsoft_silverlight/).
- Java in browsers is on life support (although it’s alive and well on servers and as the Android development language)
- Web developers have learned how to make deep content and database-created pages easy to browse and to spider

Most of the problems that sitemaps were meant to fix are no longer problems. If your website still has Flash content or Java applets, it’s time to adopt HTML5. If your content is available only by searching, you should make it browsable.

## But what about Google? sitemap.xml is required, right? It helps your PageRank, right? Link juice?

**No.**

There is no Google "bonus" for having a sitemap.xml.

**I repeat: There is no Google "bonus" for having a sitemap.xml.**

Sitemaps don’t even guarantee that Google will index those pages. As Michael Cottam wrote in his [excellent blog on sitemaps](https://moz.com/blog/xml-sitemaps):

> Probably the most common misconception is that the XML sitemap helps get your pages indexed. The first thing we’ve got to get straight is this: Google does not index your pages just because you asked nicely. Google indexes pages because (a) they found them and crawled them, and (b) they consider them good enough quality to be worth indexing. Pointing Google at a page and asking them to index it doesn’t really factor into it.

For an informational site, whether it’s small or large, no sitemap is required.

Still, most SEO audit tools will still flag a "missing" sitemap. As with other elements of a technical SEO audit, you should apply your knowledge and human judgment.


## So it's useless?

Not quite. There are a few useful jobs for the sitemap.xml.

### Managing Crawl Budget

Google is huge, but it still needs to use its resources wisely. Google allocates a certain “budget” of its GoogleBot time to sites. It doesn’t necessarily crawl every page of your site at once. It often splits the site crawl jobs into batches; I’ve seen Google take weeks to finish crawling a site. So if your site has 5,000 pages, and you recently updated a dozen, you want Google to focus this. You can update the modification dates for them in sitemap.xml, which signals to Google that it should focus its effort there.

### Trigger a Re-crawl After a Site Relaunch

If you relaunch a site and change many pages’ URLs, a sitemap tells Google “Hey, I added a bunch of new links, would you please crawl them?” Google may or may not choose to do something with that – it's a request, not a guaranteed SLA.

If you use Google as the back end site search service, doing this will (usually) help kick off a re-spider and refresh search results to point to the new content and pages. (Technically, this isn't an SEO function.)

The new Google Search Console (GSC) no longer allows you to re-crawl entire sites by submitting a single changed URL. The new GSC only indexes the single page you asked it to look at. So, if you need to have Google re-spider the whole site, it's sitemap time.

### Show a Quick Hit

There is some empirical evidence that submitting a sitemap causes Google to crawl faster and push pages into search results faster. But, the most recent evidence I’ve found for this dates back to 2011, and Google has made major changes in the past eight years.


## If you _must_ have a sitemap…

Pragmatically, sometimes you just have a stakeholder that wants a sitemap, and you can’t say no. Luckily, it's fast and easy to install a Craft, WordPress, or Drupal plug-in that generates a sitemap.xml. It won't hurt anything, and it might help your stakeholder feel more confident.

### CMS Plug-ins for Sitemap.xml files:
- Craft 3 CMS: [XML Sitemap](https://plugins.craftcms.com/sitemap)
- WordPress: [Yoast](https://yoast.com/wordpress/)
- Drupal 7 & 8: [XML Sitemap](https://www.drupal.org/project/xmlsitemap)


### So: Do sites really need a sitemap.xml?

**Almost never.** If you want to submit a bunch of changed pages for indexing, upload a new sitemap. Aside from that, it’s a harmless peace-of-mind prophylactic.

![Sitemap.xml doesn't help SEO - Change My Mind](/images/blog/blog-do-sites-need-a-sitemap.jpg)


*Originally written for and published on the Imarc.com blog at [www.imarc.com/blog/do-sites-really-need-a-sitemap-for-seo](https://www.imarc.com/blog/do-sites-really-need-a-sitemap-for-seo)*
