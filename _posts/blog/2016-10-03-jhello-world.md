---
layout: post
title: "Jhello world"
modified:
categories: blog
excerpt:
tags: []
image:
  feature:
date: 2016-10-03T15:39:55-04:00
---
### Malware uses Mars Rover code to spy on Indian-Afghani relations
Disappointingly down-to-earth Microsoft Word vulnerability exploited.

![](https://cdn.grahamcluley.com/wp-content/uploads/2016/03/mars-rover.jpeg)

A strain of malware has incorporated code used by the Mars Rover exploration robot in an attempt to spy on relations between India and Afghanistan.

Vicky Ray and Kaoru Hayashi, threat intelligence analysts with Palo Alto Networks, explain in a blog post that they identified a targeted attack on Christmas Eve last year in which an attacker - posing as the current Defense Minister of India, Mr. Manohar Parrikar - sent out a fake email to India's Ambassador to Afghanistan.

In recent years, India has helped fund Afghanistan's economic development and construction of critical infrastructure, including power plants, transportation systems, and a new parliament complex for the Afghan government.

Building off of this history, the fake email appears to commend the Ambassador for leading several development projects in Afghanistan and comes with an attachment entitled "Appreciation_letter.doc."

![](https://cdn.grahamcluley.com/wp-content/uploads/2016/03/malicious-email.jpeg)

Unfortunately, there will be no celebrating a job-well-done today. The attachment is not an appreciation letter; it's an RTF file that exploits the CVE-2010-3333 Microsoft Word vulnerability to execute a downloader, which in turn downloads the Rover Trojan.

What makes Rover unique is its use of OpenCV and OpenAL. The former is a software library that has been used by security systems, driver-less cars, and even the Mars Rover exploration robot for capturing and transmitting images, whereas the latter is a cross-platform audio API.

The malware makes use of these resources in order to take photos from the webcam and to record audio. These files are then sent to the malware authors via a command-and-control (C&C) server.

Rover also has the ability to take screenshots, log keystrokes, and copy removable drives for documents containing common file extensions.

![](https://cdn.grahamcluley.com/wp-content/uploads/2016/03/grab-screenshot.jpeg)

Researchers Ray and Hayashi observe that there is little sophisticated about the malware, but that matters little if it succeeds in stealing information:

> "Though 'Rover' is an unsophisticated malware lacking modern malware features, it seems to be successful in bypassing traditional security systems and fulfilling the objectives of the threat actor behind the campaign in exfiltrating information from the targeted victim. It is important to understand the techniques and tools being used by such threat actors to better defend and protect organizations from such threats."

Rover was involved in a targeted attack against India's Ambassador to Afghanistan, so ordinary users probably need not fear this particular malware campaign. However, they should be on the lookout for other instances of Rover and similar malware that attempts to infect their machines via fake emails.

As always, it is wise to exercise caution around suspicious messages and to refrain from opening attachments delivered to you from unknown senders.





[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll]:    http://jekyllrb.com
