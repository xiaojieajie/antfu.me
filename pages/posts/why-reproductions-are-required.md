---
title: Why Reproductions are Required
date: 2022-05-30T16:00:00Z
lang: en
duration: 9min
description: My thoughts on why reproductions are important in open source.
---

[[toc]]

If you have ever browsed the issue lists in my repos or created one, you might sometimes see I reply with the following comment and then close the issue:

<figure>
<img src="/images/issue-close-without-repro-light.png" img-light rounded-lg>
<img src="/images/issue-close-without-repro-dark.png" img-dark rounded-lg>
<figcaption>We temporarily close this due to the lack of enough information. Please provide a <a href="https://stackoverflow.com/help/minimal-reproducible-example" target="_blank">minimal reproduction</a> to reopen the issue. Thanks.</figcaption>
</figure>

I'd first say sorry if it ever makes you feel unpleasant. In this post, let me try to explain the reason behind it.

## Open Source Software is served "as-is"

First of all, let's reach a consensus about Open Source Software(OSS). If you look into the MIT License, one of the most popular licenses, you will see it contains the following statement:

> The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement.

"As is" stands that you are free to use the code, fork it, or modify it as you want with the **current state**. Meaning the authors are not responsible to fix or improve anything you might have now or in the future. Since it's free and open source, the authors or maintainers gain nothing regardless if you use it or not. There is no such thing as 24-7 customer service. Theoretically, you as a consumer, should be responsible to the code you use.

Yeah, that sounds scary. But luckily, things are not that bad in real practice. In many open source projects, we build trust between users and maintainers. Users contribute to projects by reporting issues they faced, or sharing solutions via discussions and pull requests. Maintainers spend their time reviewing, making decisions, managing releases, and doing distributions. Both users and maintainers work **voluntarily** toward the same wish - to make the software better, for everyone.

## Maintainance takes effort, a lot

Software once written, is never finished. Maintainance plays a crucial role to keep a project "alive", getting bug or security fixes on time, and being sustainable in the long run. Things like triaging issues, reviewing PRs, and discussions could take a lot of effort from maintainers. While in open source projects, the ratios of user-to-maintainer are commonly unbalanced. Many popular projects might only have one or two maintainers behind the scene. As a project grows and gains more users, the number of tasks required to maintain the project may easily go beyond one’s capacity.

<figure>
<img src="/images/github-inbox-light.png" img-light rounded-lg>
<img src="/images/github-inbox-dark.png" img-dark rounded-lg>
<figcaption>My inbox of GitHub notifications</figcaption>
</figure>

## Why Reproduction

A good [minimal reproduction](https://stackoverflow.com/help/minimal-reproducible-example) of a potential issue could greatly help maintainers to identify the root cause and land the fix quickly. Without a minimal reproduction, merely from the issue description or a screenshot, maintainers won't even know whether it's a real issue of the project or it's caused by some other factors. To identify that, maintainers might need to spend extra time to find a reproduction themselves, or dive into the giant project people shared as a "non-minimal reproduction". Hours might be spent, but what if it turns out a non-issue or unreproducible? What if there are hundreds of such issues you need to deal with?

In my opinion, **asking for minimal reproduction is asking for equity of the effort spent**. If everyone could take some time to create a minimal reproduction before opening issues, it would save maintainers hundreds of hours (or even help themselves to find user-land solutions/mistakes, then they don't even need to create the issue). A well-investigated and well-explained issue would also make maintainers more willing to spend their time and effort in return.

## Wrapping Up

As a maintainer, I appreciate all the issues and pull requests opened. And I believe it's true that some of the issues we closed without reproduction might still have real bugs that need to be fixed. But to not be overwhelmed by the notifications, maintainers need to set the priorities for handling the tasks. Keeping the number of issues in a manageable manner is one of the ways to keep the project healthy in the long run.

I believe open source is about building great stuff together, not solely on maintainers' shoulders. Wish we could make a better and healthier community together. Thanks for reading :)
