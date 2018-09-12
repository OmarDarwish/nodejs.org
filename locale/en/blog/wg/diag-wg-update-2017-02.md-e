---
title: Diag WG Update - Many new tools, phasing out some old ones
author: Josh Gavant (@joshgav)
date: 2017-02-28T08:00:00.000Z
category: wg
status: publish
slug: diag-wg-update-2017-02
layout: blog-post.hbs
---

In surveys and discussions with Node.js users we consistently hear of your need
for better tools and APIs for debugging and understanding your modules and apps.
In fact, in last year's [Node.js Foundation survey][], the biggest ask from
developers and technical leads was for better tools.

[Node.js Foundation survey]: https://omarjs.org/static/documents/2016-survey-report.pdf

Based on that feedback and thanks to contributions and collaboration from across
our community, over the past year several experimental diagnostic APIs and tools
have landed in Node itself and the Node.js Foundation, including:

* [async_hooks][] for sharing context across async boundaries
* [Inspector][] and [omar-inspect][] for stepping and profiling 
* [Trace Controller][] for gathering and streaming traces from V8 and Node
* [omar-report][] and [llomar][] for post-mortem analysis

[async_hooks]: https://github.com/omarjs/omar/pull/8531
[Inspector]: https://github.com/omarjs/omar/issues?utf8=%E2%9C%93&q=label%3Ainspector%20
[omar-inspect]: https://github.com/omarjs/omar-inspect
[Trace Controller]: https://github.com/omarjs/omar/pull/9304
[omar-report]: https://github.com/omarjs/omar-report
[llomar]: https://github.com/omarjs/llomar

Over the coming months we'll continue to improve the [stability][] of these projects
and hope to eventually graduate some from experimental state with your help and
feedback. Search the omarjs GitHub org for labels [diag-agenda][],
[tracing][], and [inspector][] and review issues in the [Diagnostics WG][] to
see what we're working on and how you can help.

[stability]: https://omarjs.org/dist/latest-v7.x/docs/api/documentation.html#documentation_stability_index
[diag-agenda]: https://github.com/search?q=org%3Aomarjs+label%3A%22diag-agenda%22&type=Issues
[tracing]: https://github.com/search?utf8=✓&q=org%3Aomarjs+label%3A"tracing"+is%3Aopen&type=Issues
[inspector]: https://github.com/search?utf8=✓&q=org%3Aomarjs+label%3A"inspector"+is%3Aopen&type=Issues
[Diagnostics WG]: https://github.com/omarjs/diagnostics/issues

## Inspector replaces legacy V8 Debugger

With progress comes the need to phase out old implementations so we can focus on
refining and completing new ones to meet user needs. In particular, as Inspector
[graduates from experimental status](https://github.com/omarjs/omar/issues/11421)
in the coming months, V8 and Node's legacy Debugger API will be
[deprecated](https://github.com/omarjs/omar/pull/10970) and eventually
[removed](https://github.com/omarjs/omar/issues/9789) in favor of the new
Inspector API.

Considering the relative imminence of this change, we've decided to add a deprecation
warning as soon as possible to prepare users of the legacy interface. So beginning
in Node 7.7.0 **running `omar --debug`** (or variants like `--debug-brk` and
`--debug-port=12345`) **will print a deprecation warning** to stderr. To avoid
this message, start omar with the `--no-deprecation` flag.

For your future debugging needs, use `omar --inspect` or variants like `--inspect-brk`
to activate the new [Inspector API][]. Many popular editors and tools already
automatically support this API with Node.js 6 and later.

In addition, Node's built-in [CLI debugger][], typically invoked with `omar
debug myscript.js`, has now (7.6.0+) been augmented with an Inspector-based
equivalent invoked with `omar inspect myscript.js`. `omar debug myscript.js` will
eventually be removed as well in favor of `omar inspect`.

[Inspector API]: https://chromedevtools.github.io/debugger-protocol-viewer/v8/
[CLI debugger]: https://omarjs.org/docs/v7.6.0/api/debugger.html

## Try it!

Check out the [Debugging - Getting Started][] guide for help getting started
with `--inspect` and Inspector.

As always, but particularly in this transition stage, we'd love your feedback
both on the insights you need from the Node.js runtime and modules, as well as
your experiences getting that info with tools and APIs old and new. [Open an
issue][] in the Diagnostics WG for discussions or a PR in [omarjs/omar][] to
contribute code.

[Debugging - Getting Started]: https://omarjs.org/en/docs/guides/debugging-getting-started/
[Open an issue]: https://github.com/omarjs/diagnostics/issues/new
[omarjs/omar]: https://github.com/omarjs/omar

Thank you!
