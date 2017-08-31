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

### New Windsor

At one point, the [Town of New Windsor](http://town.new-windsor.ny.us/) appeared to be assisting with running DNN sites for [five other towns](New%20York/New%20Windsor/002.JPG):

* [Montgomery](http://www.townofmontgomery.com/)
* [Crawford](http://www.townofcrawford.org/)
* [Blooming Grove](http://www.townofbloominggroveny.com/) - URL may have changed
* [Highlands](http://www.highlands-ny.gov/)
* [Cornwall](http://www.cornwallny.com/)

The WHOIS registrant contact for townofcrawford.org at the time of writing is Patrick Mangan, the [Deputy CITO](http://town.new-windsor.ny.us/OfficialsDepartments/InformationTechnology.aspx) of the Town of New Windsor.

There were also references to:

* [Monroe Police Department](New%20York/New%20Windsor/163.JPG), [monroepd.org](http://www.monroepd.org/)
* [The Josephine-Louise Public Library of Walden](New%20York/New%20Windsor/053.JPG), [waldenlibrary.org](http://www.waldenlibrary.org/)

The WHOIS registrant contact for waldenlibrary.org at the time of writing is Patrick Mangan of [Hudson Valley Computer Guys](http://www.hvcomputerguys.com/).

At about 10am on June 27<sup>th</sup>, requests for [backup restoration](New%20York/New%20Windsor/205.JPG) and [malware scans](New%20York/New%20Windsor/208.JPG) were sent to the hosting provider [GearHost](https://www.gearhost.com/) by Patrick Mangan. GearHost [restored a backup from June 26<sup>th</sup>](New%20York/New%20Windsor/191.JPG), though additional actions by Patrick Mangan were apparently necessary to return the site to working order.

At about 11am on June 27<sup>th</sup>, [Bonnie Becker](https://www.nytowns.org/node/1283) of the [New York State Association of Towns](https://www.nytowns.org/) [forwarded a warning](New%20York/New%20Windsor/209.JPG) from the New York State Intelligence Center and the [Multi-State Information Sharing and Analysis Center](https://www.cisecurity.org/ms-isac/) about the DNN site compromises.

At some point, the town [received an update notice for EasyDNNnews](New%20York/New%20Windsor/287.JPG), which included a claim that they had previously purchased the module. It was unclear if the module was still in use, and if so, on what site(s).

A month later, on July 27<sup>th</sup>, [an exchange](New%20York/New%20Windsor/042.JPG) between Patrick Mangan and [Mitchel Sellers](https://mitchelsellers.com/) of [Iowa Computer Gurus](https://www.iowacomputergurus.com/) details the compromise of waldenlibrary.org a few days prior, apparently leveraging the installation wizard files, and having footer text on the site contain a malicious redirect. Patrick Mangan [claimed](New%20York/New%20Windsor/051.JPG) to have deleted the install wizard files after the compromise occurred, and hoped to discuss securing the town sites a bit by phone.

The topic of securing the town sites was [discussed further](New%20York/New%20Windsor/038.JPG) on July 28<sup>th</sup>, a [phone call was scheduled](New%20York/New%20Windsor/133.JPG) for August 1<sup>st</sup> at 9am, and may have taken place [after 9:15am](New%20York/New%20Windsor/231.JPG).

At some point, [Mitchel Sellers was granted a superuser account](New%20York/New%20Windsor/151.JPG) on various sites.

On August 3<sup>rd</sup>, the [patches for Telerik and DNN GO were applied](New%20York/New%20Windsor/159.JPG). Over the following two days, there was some [discussion about attempting to upgrade DNN](New%20York/New%20Windsor/270.JPG) to 9.1.1.

## Rhode Island

### Department of Education

The Rhode Island Department of Education had [contracted](Rhode%20Island/Department%20of%20Education/RE%20DNN%20Vulnerability%20-%20Urgent%20Attention%20Required%20-2.msg) with [Envision Technology Advisors, LLC](https://www.envisionsuccess.net/) with respect to "Web Site Accessibility, Functionality and Sustainability".

Ed Giroux, the Director of RIDE's [Office of Network and Information Systems](http://www.ride.ri.gov/InsideRIDE/RIDEOffices/NetworkInformationSystems.aspx) [discussed](Rhode%20Island/Department%20of%20Education/Re%20EXTERNAL%20%20Website%20has%20been%20hacked.msg) the site being compromised at 6pm on June 26<sup>th</sup>. Kurt Huhn of the Rhode Island Division of Information Technology sent a copy of a message from the [Multi-State Information Sharing and Analysis Center](https://www.cisecurity.org/ms-isac/), which discussed the site compromises, and the vulnerable Mandeeps and EasyDNN modules.

The morning of June 27<sup>th</sup>, there was [some speculation](Rhode%20Island/Department%20of%20Education/FW%20DNN%20Vulnerability%20being%20exploited%20are%20you%20patched%20-2.msg) that [CVE-2015-2794](https://www.cvedetails.com/cve/CVE-2015-2794/) or another issue affecting the installation wizard files (such as the later bug speculated by Ars Technica) may have been to blame, but supposedly Envision had addressed those issues in June 2016.

An upgrade to DNN 9 was [scheduled for 1:30pm on June 27<sup>th</sup>](Rhode%20Island/Department%20of%20Education/DNN%20upgrade%20to%209.msg). Users were told the site would be [locked at 10:30am](Rhode%20Island/Department%20of%20Education/FW%20Website%20will%20be%20locked%20at%201030am%20-3.msg).

The evening of June 28<sup>th</sup>, [Envision shared part of a security advisory](Rhode%20Island/Department%20of%20Education/RE%20DNN%20Vulnerability%20-%20Urgent%20Attention%20Required.msg) they received in which it was suggested that multiple files related to Mandeeps modules be deleted. Envision added that it was "likely" this was related to the site compromise. The deletion happened by late morning June 29<sup>th</sup>.
