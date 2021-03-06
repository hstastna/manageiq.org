---
title: Sprint 51 review - January 4, 2017
author: cybette
date: 2017-01-06 11:15:19 UTC
tags: sprints
comments: true
published: true
---

Welcome to the first sprint review of 2017! It was a relatively succinct meeting, so I'll try to keep this short and sweet. First, a couple of news items in case you missed them:

* Just before the holidays, we released [ManageIQ Euwe GA](/blog/2016/12/manageiq-euwe-ga-announcement/). Onwards to [Fine](/blog/2016/11/announce_f_name/)!
* Length of ManageIQ Sprints change from [3 weeks to 2 weeks](/blog/2017/01/schedule-change-3-week-sprints-to-2-week-sprints/), with immediate effect.

During this 4-week sprint filled with holiday spirit, we sprinkled in 249 pull requests in the [main repo](https://github.com/ManageIQ/manageiq) and 439 PRs [overall](https://github.com/manageiq). While the total number is smaller than usual, there are more enhancement PRs than the previous sprint. But before we touch on some of these enhancements, here's an important change in the ManageIQ repository distribution.

Major effort went into the creation of 4 new repos (splitting them from the main repo): Classic UI, Content (Automate Domain), PGLogical Replication, and Design. The one with the biggest impact is Classic UI, which frequently took the largest slice of the main repo PR pie. If you work on UI, be sure to read the [discussion on the talk forum](http://talk.manageiq.org/t/new-split-repo-manageiq-ui-classic/1983).

Other repos on the splitting block for this year include Database Schema, Automate Engine, REST API, and each of the Providers. This is the first phase of transforming ManageIQ from a monolithic app to a platform, with each module having its own test suites and services, ensuring code coverage and quality throughout development. Discuss and stay informed about the progress on [ManageIQ Talk](http://talk.manageiq.org/).

In Classic UI, columns displaying virtual CPU and memory values for Cloud Providers are added, along with a new menu item to provision a Floating IP in Network. Notifications of asynchronous operations are now shown for Middleware. Several screens have been moved from Classic UI to Service UI, such as approval requests for admins, view service / VM details, and list / create / remove service catalogs.

New Chargeback features include support for fixed and allocated costs without metrics, and arbitration logic for multiple assigned rates. On the Automate side, enhanced messaging has been extended to Ansible and Cloud Provisioning, and importing Automate modeling from the UI now honors the tenant.

For the VMware vCloud provider, XLAB added the ability to specify VM attributes when deploying vApps. As for providers in general, we made a big step with the new Provider Generator, which was [proposed](https://www.youtube.com/watch?v=i5ZuTKFQqJ8) in last year's Design Summit. With a single line of command, `rails generate provider ProviderName` will generate the scaffolding for a provider. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/2iRkB_eKb44" frameborder="0" allowfullscreen></iframe>

Here's the [Sprint 51 review meeting video](https://www.youtube.com/watch?v=2iRkB_eKb44), and the corresponding timestamps for each section:

* Sprint Statistics (Oleg Barenboim) -[0:52](https://youtu.be/2iRkB_eKb44?t=52)
* Community Update (Carol Chen) -[7:51](https://youtu.be/2iRkB_eKb44?t=471)
* Classic UI (Dan Clarizio) -[11:38](https://youtu.be/2iRkB_eKb44?t=698)
* Service UI (Chris Kacerguis) -[13:50](https://youtu.be/2iRkB_eKb44?t=830)
* Providers (Greg Blomquist) -[16:35](https://youtu.be/2iRkB_eKb44?t=995)
* Automate (Greg McCullough) -[18:55](https://youtu.be/2iRkB_eKb44?t=1135)
* Platform (Gregg Tanzillo) -[21:43](https://youtu.be/2iRkB_eKb44?t=1303)
* API (Alberto Bellotti) -[25:20](https://youtu.be/2iRkB_eKb44?t=1520)
* Discussion -[28:55](https://youtu.be/2iRkB_eKb44?t=1735)

Delve into some specific PRs with these 3 installments of “Last Week in ManageIQ”:

* [Provider generator, pglogical upgrades, and Chen primes!](/blog/2016/12/last-week-in-manageiq-provider-generator-pglogical-chen-primes/) - by [Chris Arcand](https://twitter.com/chrisarcand) 
* [Armor like Tenfold Regions Hashes](/blog/2016/12/last-week-in-manageiq-armor-like-tenfold-regions-hashes/) - by [Drew Uhlmann](https://github.com/d-m-u)
* [A brand new Euwe](/blog/2017/01/last-week-in-manageiq-a-brand-new-euwe/) - by [Julian Cheal](http://juliancheal.co.uk/)

As mentioned above, the next sprint will be in 2 weeks instead of 3, so Sprint 52 review will be on January 18, 2017 @ [7:30 PST/10:30 EST/15:30 GMT](http://www.timeanddate.com/worldclock/fixedtime.html?msg=ManageIQ+Sprint+52+review&iso=20170118T1530). Join in the ManageIQ Sprint meeting via [Bluejeans](https://bluejeans.com/5927041376/) and import the updated [ManageIQ community calendar](https://calendar.google.com/calendar/embed?src=contact%40manageiq.org) to be notified about this and future Sprint reviews!

### [Sprint 51 Slide deck](http://www.slideshare.net/ManageIQ/sprint-51-review)

<iframe src="//www.slideshare.net/slideshow/embed_code/key/48gZvEYdGZYudf" width="510" height="420" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe>

