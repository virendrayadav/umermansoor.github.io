---
layout: post
title: If Your Site Isn't Using HTTPS, You Are Doing It Wrong
comments: True
excerpt_separator: <!--more-->
---

We live in a day and age where we simply cannot *take our right to privacy for granted*. When we communicate over **unprotected channels, we expose our messages to everyone who happens to be along the way**: The WiFi hotspots, corporate IT providers, ISPs, cloud providers, can listen in to our communication. We leave a trail of digital footprints behind. When aggregated, it can reveal information about ourselves. Eavesdroppers and intruders can make inferences about our behaviors and intentions: ISPs can determine what types of news stories we are interested in, employers can monitor our activities even on personal devices at work, look at our searches, see our messages, all when we communicate over unprotected channels.

![Privacy]({{ site.url }}/img/privacy.jpg)

<!--more-->

Google has been [urging site owners to switch to HTTPS](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/why-https) for many years now. They started using HTTPS as a [ranking indicator](https://webmasters.googleblog.com/2014/08/https-as-ranking-signal.html) for their search results. To tighten the screws, Chrome, starting with version 56 that is coming soon, will start **showing "not secure" alerts on sites that collect login or credit card information over HTTP**. Firefox will also [start displaying a red icon in the address bar as well as an in-context warning](https://blog.mozilla.org/security/2017/01/20/communicating-the-dangers-of-non-secure-http/) for pages that ask users to login over HTTP.

![Firefox]({{ site.url }}/img/firefoxwarning.png)

While I don't know the real reason that compel Google to drive the HTTPS campaign, it's a great direction for the future of the web, a direction that we should all support.

So how do you make your website secure? It's way easier to secure sites with HTTPS these days than it used to be. In the past, obtaining a digital certificate that is required for HTTPS required paperwork and hundreds of dollars. This is no longer the case. **[Let's Encrypt](https://letsencrypt.org/) is a certificate authority that provides FREE certificates to anyone**. It's backed by organizations such as Mozilla, Facebook and Google to name a few. Let's Encrypt makes it possible for anyone to have an HTTPS website for free. As an alternative, if you host your servers on the AWS, [Certificate Manager](https://aws.amazon.com/blogs/aws/new-aws-certificate-manager-deploy-ssltls-based-apps-on-aws/) provides free certificates and handle certificate renewals as an added bonus.

Getting an HTTPS-enabled website is easier (and cheaper) now than ever. If you are concerned that HTTPS slows things down, [think again](https://istlsfastyet.com/). **HTTPS can even be [faster](https://www.troyhunt.com/i-wanna-go-fast-https-massive-speed-advantage/) than HTTP**.

![HTTP vs HTTPS]({{ site.url }}/img/httpvshttps.jpg)

I didn't intentionally touch upon security threats to unencrypted traffic since they are well known to most people. The privacy aspects, unfortunately, aren't as well known.

I would also like to make a quick announcement: **starting today, all traffic to my blog is 100% fully encrypted and secured using HTTPS**. I enabled HTTPS without spending a single penny and the whole process took less than an hour. If you have a website that isn't using HTTPS yet, what are you waiting for?
