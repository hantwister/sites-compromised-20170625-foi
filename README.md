# sites-compromised-20170625-foi
A repo for responses to freedom of information inquiries related to various DNN site compromises on about June 25<sup>th</sup>, 2017

## Background
Around June 25<sup>th</sup>, [various](http://www.cnn.com/2017/06/25/politics/kasich-hack-isis/index.html) [news](http://thehill.com/policy/cybersecurity/339395-kasichs-website-hacked-with-what-appears-to-be-pro-isis-messages) [sites](http://www.chicagotribune.com/news/nationworld/ct-ohio-government-websites-hacked-islamic-state-20170625-story.html) began reporting on various city and state government sites being compromised and displaying a pro-ISIS message.

Ars Technica [reported](https://arstechnica.com/information-technology/2017/06/ohio-gov-kasichs-website-dozens-of-others-defaced-using-year-old-exploit/) that the sites that were reported compromised all used old versions of [DNN (previously known as DotNetNuke)](http://www.dnnsoftware.com/community/download), and speculated that [a vulnerability from May 2016](https://www.cisecurity.org/advisory/vulnerability-in-dotnetnuke-dnn-content-management-system-could-allow-for-unauthorized-access/) may have been to blame. With respect to the May 2016 vulnerability, it was unclear if the system administrators for the compromised sites had taken the suggested mitigation steps (remove or block access to certain files only used during installation and updates) in lieu of updating their installation.

It was noteworthy that [a critical update for DNN was released on June 21<sup>st</sup>, 2017](http://www.dnnsoftware.com/community-blog/cid/155436/critical-security-update--june-2017), days prior to these compromises; it was also unclear if the system administrators for the compromised sites had installed this very recent update, or if the vulnerability addressed by the update played any role in the compromises.

DNN described the June 21<sup>st</sup>, 2017 update as addressing a flaw in a third-party component used by DNN. Carnegie Mellon University's CERT Division [publicly associated](https://www.kb.cert.org/vuls/id/TNOY-APDS9B) the DNN update with Progress Software's [Telerik UI for ASP.NET AJAX library](http://www.telerik.com/products/aspnet-ajax.aspx) and [CVE-2017-9248](http://www.telerik.com/support/kb/aspnet-ajax/details/cryptographic-weakness). The Telerik library also had an update on June 21<sup>st</sup>, 2017, with [the release notes mentioning "security improvements"](http://www.telerik.com/support/whats-new/aspnet-ajax/release-history/ui-for-asp-net-ajax-r2-2017-sp1-version-2017-2-621).

In an effort to clarify what vulnerabilities may have been involved in the aforementioned compromises, and how the respective system administrators handled the compromises, requests were sent to various city and state governments for e-mails containing one of several keywords, such as DNN.

## New York

### Cornwall

[Renata McGee](http://www.cornwallny.com/Departments/Town-Clerk), the Town Clerk, [left a voicemail](New%20York/Cornwall/20170814-1227-McGee.mp3) stating that the Town of New Windsor handled IT services for them and several other municipalities.
