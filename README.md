# sites-compromised-20170625-foi
A repo for responses to freedom of information inquiries related to various DNN site compromises on about June 25<sup>th</sup>, 2017

## Background
Around June 25<sup>th</sup>, [various](http://www.cnn.com/2017/06/25/politics/kasich-hack-isis/index.html) [news](http://thehill.com/policy/cybersecurity/339395-kasichs-website-hacked-with-what-appears-to-be-pro-isis-messages) [sites](http://www.chicagotribune.com/news/nationworld/ct-ohio-government-websites-hacked-islamic-state-20170625-story.html) began reporting on various city and state government sites being compromised and displaying a pro-ISIS message.

Ars Technica [reported](https://arstechnica.com/information-technology/2017/06/ohio-gov-kasichs-website-dozens-of-others-defaced-using-year-old-exploit/) that the sites that were reported compromised all used old versions of [DNN (previously known as DotNetNuke)](http://www.dnnsoftware.com/community/download), and speculated that [a vulnerability from May 2016](https://www.cisecurity.org/advisory/vulnerability-in-dotnetnuke-dnn-content-management-system-could-allow-for-unauthorized-access/) may have been to blame. With respect to the May 2016 vulnerability, it was unclear if the system administrators for the compromised sites had taken the suggested mitigation steps (remove or block access to certain files only used during installation and updates) in lieu of updating their installation.

It was noteworthy that [a critical update for DNN was released on June 21<sup>st</sup>, 2017](http://www.dnnsoftware.com/community-blog/cid/155436/critical-security-update--june-2017), days prior to these compromises; it was also unclear if the system administrators for the compromised sites had installed this very recent update, or if the vulnerability addressed by the update played any role in the compromises.

DNN described the June 21<sup>st</sup>, 2017 update as addressing a flaw in a third-party component used by DNN. Carnegie Mellon University's CERT Division [publicly associated](https://www.kb.cert.org/vuls/id/TNOY-APDS9B) the DNN update with Progress Software's [Telerik UI for ASP.NET AJAX library](http://www.telerik.com/products/aspnet-ajax.aspx) and [CVE-2017-9248](http://www.telerik.com/support/kb/aspnet-ajax/details/cryptographic-weakness). The Telerik library also had an update on June 21<sup>st</sup>, 2017, with [the release notes mentioning "security improvements"](http://www.telerik.com/support/whats-new/aspnet-ajax/release-history/ui-for-asp-net-ajax-r2-2017-sp1-version-2017-2-621).

Another source [reported](https://mitchelsellers.com/blogs/2017/06/30/june-2017-dnn-evoq-and-module-security-summary) that, in addition to the update for DNN itself, critical updates were recently released for various modules, including several by [Mandeeps](https://www.mandeeps.com/company/news/critical-security-update---june-2017), some by [DNN GO](https://www.dnngo.net/), and one by [EasyDNN](http://www.easydnnsolutions.com/). Likewise, it was unclear if any of these modules played a role in the compromises.

In an effort to clarify what vulnerabilities may have been involved in the aforementioned compromises, and how the respective system administrators handled the compromises, requests were sent to various city and state governments for e-mails containing one of several keywords, such as DNN.

## New York

### Cornwall

[Renata McGee](http://www.cornwallny.com/Departments/Town-Clerk), the Town Clerk, [left a voicemail](New%20York/Cornwall/20170814-1227-McGee.mp3) stating that the Town of New Windsor handled IT services for them and several other municipalities.

## Rhode Island

### Department of Education

The Rhode Island Department of Education had [contracted](Rhode%20Island/Department%20of%20Education/RE%20DNN%20Vulnerability%20-%20Urgent%20Attention%20Required%20-2.msg) with [Envision Technology Advisors, LLC](https://www.envisionsuccess.net/) with respect to "Web Site Accessibility, Functionality and Sustainability".

Ed Giroux [discussed](Rhode%20Island/Department%20of%20Education/Re%20EXTERNAL%20%20Website%20has%20been%20hacked.msg) the site being compromised at 6pm on June 26<sup>th</sup>. Kurt Huhn of the Rhode Island Division of Information Technology sent a copy of a message from the [Multi-State Information Sharing and Analysis Center](https://www.cisecurity.org/ms-isac/), which discussed the site compromises, and the vulnerable Mandeeps and EasyDNN modules.

The morning of June 27<sup>th</sup>, there was [some speculation](Rhode%20Island/Department%20of%20Education/FW%20DNN%20Vulnerability%20being%20exploited%20are%20you%20patched%20-2.msg) that [CVE-2015-2794](https://www.cvedetails.com/cve/CVE-2015-2794/) or another issue affecting the installation wizard files (such as the later bug speculated by Ars Technica) may have been to blame, but supposedly Envision had addressed those issues in June 2016.

An upgrade to DNN 9 was [scheduled for 1:30pm on June 27<sup>th</sup>](Rhode%20Island/Department%20of%20Education/DNN%20upgrade%20to%209.msg). Users were told the site would be [locked at 10:30am](Rhode%20Island/Department%20of%20Education/FW%20Website%20will%20be%20locked%20at%201030am%20-3.msg).

The evening of June 28<sup>th</sup>, [Envision shared part of a security advisory](Rhode%20Island/Department%20of%20Education/RE%20DNN%20Vulnerability%20-%20Urgent%20Attention%20Required.msg) they received in which it was suggested that multiple files related to Mandeeps modules be deleted. Envision added that it was "likely" this was related to the site compromise. The deletion happened by late morning June 29<sup>th</sup>.
