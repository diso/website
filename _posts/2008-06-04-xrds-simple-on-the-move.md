---
layout: post
title: XRDS-Simple On The Move
author: Steve Ivy
---

*[DiSo][] is built on the idea of implementing social networking concepts on
existing standards where possible. One of those standards is [XRDS Simple][], a
service description and discovery format that is a part of several recent and
upcoming standards including OpenID and OAuth.*

[DiSo]: http://diso-project.org/
[XRDS Simple]: http://xrds-simple.net/core/1.0/


Since last week, when I released the first version of [XRDS-Simple for Movable
Type][], there's been some more movement in the implementation space:

 - [James Walker][] [announced][] a plugin for [Drupal][] that works similarly
   to Stephen's WordPress plugin and my own MT plugin - it provides a framework
   for apps to register services to be advertised in the XRDS doc. We now have

 - [Byrne Reese][] kindly helped me [re-package the MT plugin][] for better
   distribution (per MT standard practice), then went a step further and
   [contributed some code improvements][] to make it play more nicely with Yahoo's
   OpenID implementation.

[XRDS-Simple for Movable Type]: http://redmonk.com/archives/2008/05/27/xrds-simple-for-movable-type/
[James Walker]: http://www.walkah.net/
[announced]: http://groups.google.com/group/diso-project/browse_thread/thread/87425b545ec043ad
[Drupal]: http://drupal.org/
[Byrne Reese]: http://www.majordojo.com/
[re-package the MT plugin]: http://code.google.com/p/diso/source/detail?r=254
[contributed some code improvements]: http://code.google.com/p/diso/source/detail?r=256


There's also talk of rolling OpenID delegation (currently one of the most
common use of XRDS) into a couple of the plugins, and we're also on the lookout
for more services that are using, might use, or should be using XRDS for
service discovery. We (and by "we" I mean the [DiSo][] community) are also looking
for XRDS parser implementations that can be used in integration and interop
testing. Some brief Googling turned up parsers in:

 - [Python][] (from mr topf)
 - [Ruby][] (elc tech)

[Python]: http://mrtopf.de/blog/plone/planetplone/announcing-pydataportability-01-technical/
[Ruby]: http://www.elctech.com/blog/dataportability-xrds


If you've got pointers to other implementations (providing or consuming), or
other thoughts, hit us up in the comments.

*Update*: In doing [some reading][] it looks like a working [Yadis][] parser
(like those found in [several][] [OpenID][] [implementations][]) may also work
for parsing the XRDS-Simple output by these generators. Any
confirmation/corrections are welcome.

[some reading]: http://www.hueniverse.com//hueniverse//2008//03//putting-xrds-si.html
[Yadis]: http://yadis.org/wiki/Main_Page
[several]: http://code.sixapart.com/trac/openid/browser/branches/openid2/perl/Net-OpenID-Consumer/lib/Net/OpenID/Yadis.pm
[OpenID]: http://www.openidenabled.com/python-openid/
[implementations]: http://openidenabled.com/ruby-openid/
