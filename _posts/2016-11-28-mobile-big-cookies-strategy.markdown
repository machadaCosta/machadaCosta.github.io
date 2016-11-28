---
layout: post
title:  "Big Cookie Strategy"
date:   2016-11-28
author: Macha Da Costa
category: mobile
tags: [mobile development, big cookie strategy]
excerpt: This post is about the Big Cookie Strategy for exchange between server and mobile.
permalink: /mobile-big-cookie-strategy/
---

Big Cookie Strategy was created to optimize exchange between a mobile application and a server.
 

## What is Big Cookie Strategy ?

![Big Cookie Strategy in Mobile Development]({{ site.baseurl }}/img/big-cookie-strategy.png)
<i class="fa fa-copyright" aria-hiden="true"></i> by [CHILLCODING](https://www.chillcoding.com) with [fontawesome](http://fontawesome.io/cheatsheet/)

<i class="fa fa-list" aria-hiden="true"></i> Step by step:

1. Verify that connection is available on mobile ( <i class="fa fa-exclamation-triangle" aria-hiden="true"></i> <i class="fa fa-plane" aria-hiden="true"></i> )
2. Ask needed data to server with the connectivity state in user agent (<i class="fa fa-exchange" aria-hiden="true"></i> )
3. Receive prefetch* data from server ( <i class="fa fa-database" aria-hiden="true"></i> (<i class="fa fa-signal" aria-hiden="true"></i>) )

*Belonging to the mobile connectivity state, server send data set of different size

For instance, here is a data set proposal in terms of connectivity:

| Connectivity | Data set |
| ---------- | :--------|
| <i class="fa fa-signal" aria-hiden="true"></i> Edge | Info since one or two hour |
| 3G or 4G | Info since 3 days |
| <i class="fa fa-wifi" aria-hiden="true"></i>Wifi | Info since 15 days | 



####Resources :

* [Android - Data Transfert by Gerardnico](http://gerardnico.com/wiki/android/data_transfer)
* [Efficient data transfer in Android slides](http://www.slideshare.net/CotapEng/efficient-data-transfer-tech-talk)
* [A Call for More Energy-Efficient Apps](http://www.research.att.com/articles/featured_stories/2011_03/201102_Energy_efficient?fbid=HZjMhQoG88-)
