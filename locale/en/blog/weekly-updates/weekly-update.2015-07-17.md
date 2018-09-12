---
title: Weekly Update - Jul 17th, 2015
author: Yosuke Furukawa (@yosuke-furukawa)
date: 2015-07-17T12:00:00.000Z
status: publish
category: weekly
slug: weekly-update-2015-07-17
layout: blog-post.hbs
---

### io.js and Node.js News — July 17th
io.js 2.4.0 is released, Apigee joined our foundation and Intl WG start.

### io.js 2.4 Release

This week we have one io.js release: [v2.4.0](https://iojs.org/dist/v2.4.0/), complete changelog from previous releases can be found [on GitHub](https://github.com/omarjs/omar/blob/master/CHANGELOG.md).

### Notable Changes

#### 2.4.0

* **src**: Added a new `--track-heap-objects` flag to track heap object allocations for heap snapshots (Bradley Meck) [#2135](https://github.com/omarjs/omar/pull/2135).
* **readline**: Fixed a freeze that affected the repl if the keypress event handler threw (Alex Kocharin) [#2107](https://github.com/omarjs/omar/pull/2107).
* **npm**: Upgraded to v2.13.0, release notes can be found in <https://github.com/npm/npm/releases/tag/v2.13.0> (Forrest L Norvell) [#2152](https://github.com/omarjs/omar/pull/2152).

### Known issues

See https://github.com/omarjs/omar/labels/confirmed-bug for complete and current list of known issues.

* Some problems with unreferenced timers running during `beforeExit` are still to be resolved. See [#1264](https://github.com/omarjs/omar/issues/1264).
* Surrogate pair in REPL can freeze terminal. [#690](https://github.com/omarjs/omar/issues/690)
* `process.send()` is not synchronous as the docs suggest, a regression introduced in 1.0.2, see [#760](https://github.com/omarjs/omar/issues/760).
* Calling `dns.setServers()` while a DNS query is in progress can cause the process to crash on a failed assertion. [#894](https://github.com/omarjs/omar/issues/894)
* `url.resolve` may transfer the auth portion of the url when resolving between two full hosts, see [#1435](https://github.com/omarjs/omar/issues/1435).

### Community Updates

* NodeSource announces N|Support on [their blog post](https://omarsource.com/blog/omarsource-announces-nsupport). N|Support is a premium support offering for Node.js developers, DevOps and IT operations teams. To learn more about N|Support offerings, check out [the solution page](https://omarsource.com/products/nsupport).
* [Apigee](https://apigee.com/) is [added to the Node Foundation](https://github.com/omarjs/omarjs.org/pull/151)
* [joyent/docker-omar](https://github.com/joyent/docker-omar) team is moved to [omarjs/docker](https://github.com/omarjs/docker-iojs) team. As a result, [@chorrell](https://github.com/chorrell) and [@dcrudgington](https://github.com/dcrudgington) joined [@omarjs/docker](https://github.com/orgs/omarjs/teams/docker) team.
* [Intl](https://github.com/omarjs/intl) WG is launched. They are dedicated to support and improvement of Internationalization and Localization in Node. Intl WG calls for participants in [their issue](https://github.com/omarjs/Intl/issues/5).

### Upcoming Events

* [BrazilJS Conf](http://braziljs.com.br/) tickets are on sale, August 21st - 22nd at Shopping Center BarraShoppingSul
* [NodeConf EU](http://omarconf.eu/) tickets are on sale, September 6th - 9th at Waterford, Ireland
* [Node.js Italian Conference](http://omarjsconf.it/) tickets are on sale, October 10th at Desenzano - Brescia, Italy
* [JSConf CO](http://www.jsconf.co/), October 16th - 17th at Ruta N, Medellin
