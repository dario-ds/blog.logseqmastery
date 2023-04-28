---
title: "Logseq vs Obsidian - which PKM tool should you use?"
date: 2023-04-19T10:36:00Z
draft: false
description: "In an era of information overwhelm, these two tools are leading the charge in helping users manage their personal knowledge."
summary: "In an era of information overwhelm, these two tools are leading the charge in helping users manage their personal knowledge."
tags: ["comparison", "Obsidian","PKM"]
categories: ["Thought pieces"]
weight: 1
cover:
    image: "/obsidian.png"
---

## Introduction

Logseq and Obsidian are two of the most popular note-taking tools on the market, helping users manage their personal information in a more structured and efficient way, all in a single interface. This blog post will provide an in-depth comparison of the two tools, highlighting their similarities, differences, and strengths, and ultimately highlight why I chose Logseq over Obsidian.

Some quick disclaimers: this post doesn't get into the details of personal knowledge management or the workings and benefits of linked databases. Instead, the focus will be on providing a clear comparison of Logseq and Obsidian. As a seasoned Logseq user with over two years of experience, I must also acknowledge that I have a natural affinity for the tool. While I have experimented with Obsidian occasionally during this period, I wouldn't classify myself as an expert. I also offer a personal knowledge management course using Logseq, which creates a financial incentive to recommend Logseq. This is a potential conflict of interest that I want to be transparent about.

With all that out the way, it's helpful to look at how the tools are similar to provide a point of departure for the comparison.

---

## Similarities between the tools

- **Fundamental concepts:** Both Logseq and Obsidian are built on graph databases that utilise bi-directional linking to create connections between different pieces of information. They share a similar hypertext-style interface that enables users to access information quickly by clicking on links.
- **File storage:** Both Logseq and Obsidian prioritise local-first storage, whilst offering a 'Sync' option to support multi-device usage. They both work on a backend of Markdown files stored locally on your computer (Logseq also supports OrgMode text files). To access Logseq Sync, you can contribute a minimum of $5 per month on the [Open Collective platform](https://opencollective.com/logseq). Obsidian Sync is available through the [Obsidian website at a cost of $10 per month](https://obsidian.md/sync).
- **Operating systems and mobile apps:** Both Logseq and Obsidian support Windows, Linux, and macOS, and they both have mobile apps for iOS and Android. However, you must download the [Android app for Logseq from GitHub](https://github.com/logseq/logseq/releases/), as it is not available on the Google Play store.
- **Transclusion of information:** (references and embeds) Both tools enable you to display or embed original content from one location within another location, with a direct reference to the source material.
- **Extensibility:** Both Logseq and Obsidian have a robust plugin environment that allows users to add custom features on top of the base feature set.
- **Community:** Both tools have large communities on Discord, providing helpful resources for users to discuss their workflows and troubleshoot challenges.
- **Pricing:**  Both tools are free forever for personal use. There are are some features which can be purchased on a subscription basis (e.g., Obsidian has a Publish feature which is discussed further on)

Given the numerous similarities, one might wonder why users tend to have strong preferences for one tool over the other. There is one key difference that divides opinion. Before we get there, it is important to acknowledge a common objection raised in comparisons between the tools. Obsidian users often point to the availability of plugins to achieve similar functionality for features in Logseq. The focus of this post is on the 'out-of-the-box' functionality, which is how most new users typically engage with these tools.

---

## The major difference between the tools

**Logseq is a block-based outliner**, allowing you to organise information into a tree-like structure using bullet-points. You can think of it as a mind-map, but for text. This allows users to quickly structure and add hierarchy to their information by indenting information, and to also move quickly between different branches of information.

Users can collapse and expand indented blocks, hiding information they're not working on and therefore don't need to see. You can also zoom into and out of different levels quickly, to focus on only the content that you want to work with. Blocks can also be easily moved around the user interface by dragging and dropping using the mouse, or by using keyboard shortcuts.

Another crucial aspect of outliners is the **inheritance of linked relationships**. When a block is indented underneath another block that has links or tags, the indented block will inherit all those relationships. Rather than relying on folders for organising information, you can use a top-level block with a tag, and store related information in blocks indented beneath it. This approach provides a streamlined method for organising information and retrieving it efficiently, without the friction of questioning "where do I store it?" or "where do I go to find it?".

In contrast to the outliner approach, **Obsidian is a page-based application that functions like a long-form text editor**, similar to a Microsoft Word document. The key advantage over traditional word processors is the instant searchability of all files and folders, as well as seamless linking between different pieces of information. 

The benefit of the block-based approach over the page-based approach may appear trivial to some, but I've found it to be an impossible gap to bridge in Obsidian. To my earlier point, Obsidian can accomplish some of Logseq's outliner functionality using plugins, but it is not primarily an outliner at its core. However, Obsidian does have some major benefits over Logseq.

---

## Obsidian's major benefits

- **Markdown compatibility:** Whilst Logseq uses Markdown files, they are not 100% compatible with other programs.  Logseq strips out blank lines and doesn't allow for multiple headings in a single block. If you collapse your high level blocks, you'll also be presented with `collapsed:: true` metadata through your database. Obsidian uses 'vanilla' markdown. This makes it excellent for long form writing and ease of publishing. In fact, I edited the final version of this post in Obsidian once I'd stripped away the outlines.
- **Speed / performance**: One of the major benefits of using Obsidian is its speed. Indexing your graph and navigating to different pages is lightning quick. This was demonstrated in [the speed test](https://www.goedel.io/p/tft-performance-interim-results) conducted at the beginning of last year by Alexander Rink, which showed that Obsidian was able to import a large number of files in just a few seconds. Additionally, navigating between pages and using the graph view in Obsidian is also quicker than Logseq.
{{< figure src="/comparison.jpg" alt="My image" caption="Importing files into different TfTs - Alexander Rink, Jan 2022." class="center" >}}

- **Page-based model offers familiarity:** For those accustomed to files and folders (most people, really) Obsidian's interface allows you to stick to that paradigm, whilst introducing powerful database features.
- **Extensive plugin environment:** There is a plugin for almost every requirement, and users can even combine plugins to create tailored workflows. This flexibility enables individuals to customise their experience according to their needs. Another key distinction compared to Logseq is the differentiation of 'Core' and 'Community' plugins. Core plugins receive support from Obsidian's development team, ensuring their ongoing maintenance and optimal performance. However, this doesn't diminish the value of Community plugins, which can also be excellent additions.
- **Highly customisable nature:** For those well-versed in the Obsidian environment, the possibilities for configuration are endless.
  - *Side note: This level of customisation can also be seen as a drawback. Content creators using Obsidian often have unique configurations, which can cause confusion for others. Certain functionality only works in certain themes, which impacts the resilience of the program. The individual plugins each have their own custom settings, which can lead to an overwhelming number of options to navigate and consider.*
- **Performant graph view:** The graph view in Obsidian is more refined than Logseq, and also quicker to navigate. Users can customise their graph view's appearance by adjusting colours, node sizes, link styles, and more to suit their preferences. In general, Obsidian's graph view feels more usable than Logseq's.
- **In-house 'Publish' feature:** Many PKM users require solutions for publishing their databases as online wikis or knowledge bases. Obsidian has an [in-house publishing solution available for $8/month](https://obsidian.md/publish) to meet their needs.
- **Larger user base and community:** Having a larger community means you'll find more plugins to choose from, more content creators to help you maximise your use of the tool, and also more people on the forum to lend a hand if you need help or advice.

Obsidian clearly has a few feathers in its cap, and it's sizeable user base is justified. Despite this, Logseq brings a unique set of advantages to the table in addition to being an outliner, making it an attractive option in its own right.

---

## Logseq's major benefits

- **More native functionality 'out of the box':** Logseq has basic query and task management functionality built-in to the application. The interface also allows users to easily access linked references at the bottom of the main and side panels—a handy feature in a linked database.
- **Open-source development:** Logseq is an open-source project. Although there is a core development team driving the majority of development, you can still contribute to the development of the application. This also ensures longevity of the application. If the development team were to disappear overnight, one would still be able to download the latest version of Logseq from GitHub (and theoretically create a fork if you'd like to continue the development)
- **Enablement of block-based workflows**: I think it's worthwhile to again emphasise the merits of block-based workflows for those who may skim through the article. Outliners provide a streamlined tool to quickly input and organise information for efficient retrieval later. They allow you to deal with multiple levels of context at a time, quickly expanding, collapsing or focusing in on a particular set of blocks. They also allow for easy navigation and manipulation of information in a hierarchy.
- **More intuitive user interface**: Logseq's interface can be considered more intuitive due to its consistent appearance across various themes. The interface features a left sidebar for navigation and "Favourite" and "Recent" pages, and two panels for accessing information with the main panel and the right sidebar. Additionally, Logseq's linked references are easier to navigate. Regardless of the panel you are using, there is always a clear visual indication of the source of the information (via breadcrumbs) or linked content.
- **Opinionated "journal first" approach:** While this may seem like a small detail, it encourages a new way of working where you begin with your daily journal as a starting point and use it as a 'scratch pad'. Every time you open Logseq, you are greeted with your daily journal page by default. This feature mimics a physical A5 annual calendar, making it easy to jot down your thoughts quickly without worrying about where to store them. You can then organise them for efficient future retrieval by adding hierarchy and linking. This approach helps users enhance their workflows over time.

---

## Verdict: Why I chose Logseq over Obsidian

Both Obsidian and Logseq offer a diverse range of features that make them excellent tools for personal knowledge management. Ultimately, personal preference will play a significant role in determining the ideal tool for you. It is **\*_personal_\*** knowledge management, after all.

For me, Logseq's outliner DNA provides a familiar interface and powerful functionality. I started my personal knowledge management journey using Roam Research, a block-based outliner similar to Logseq. It became too expensive to justify given my limited understanding at the time, so I started looking for a replacement.

I found Obsidian first, but didn't grasp the way it worked. I was looking for the familiar feel of Roam Research, which by that point I'd spent a few months getting to grips with. I was also confused by the local storage of files, as Roam Research was a cloud-based web-app.

But then I discovered Logseq, and it bridged the two worlds for me, seamlessly merging an outliner application with local storage. Most importantly, it worked **out of the box**, offering powerful, (fairly) beginner-friendly functionality without the need for plugins and customisation. After about a month, I was hooked, and the rest is history.

It's worth noting that this isn't a "winner-takes-all" comparison. Both tools have their strengths, and if you can't decide, it's possible to use both tools simultaneously, as they work on the same backend of Markdown files. However, to reap greater long-term benefits, it's advisable to select one tool and use it consistently.

Ultimately, the goal is to develop a robust and personalised knowledge management system to support you, and the real trick is to get started sooner than later. I wish you the best of luck.

---

## Further resources on Logseq vs Obsidian

- [How to get started in Logseq - analogue model of blocks and pages](https://youtu.be/ZtRozP8hfEY)
- [Battle Royale: Obsidian vs Logseq - Which is Better?](https://tfthacker.substack.com/p/battle-royale-obsidian-vs-logseq)
- [TfT Performance: Interim Results](https://www.goedel.io/p/tft-performance-interim-results)
- [Quick Tip: Outlining in Obsidian](https://thesweetsetup.com/outlining-in-obsidian/)

---

## Obsidian plugins you can use to mimic Logseq

I have been cautious in my adoption of plugins. Logseq has this disclaimer when you activate plugins:	
  
>_Plugins can access your graph and your local files, issue network requests. They can also cause data corruption or loss. We're working on proper access rules for your graphs. Meanwhile, make sure you have regular backups of your graphs and only install the plugins when you can read and understand the source code._

The same is true for Obisidian. Plugins introduce a third-party risk, so you need to do your own homework. This is not meant to scare anyone. There are some trusted, credible plugin developers across both communities, although it's worthwhile to consider the risks. If you're looking for some plugins to help achieve a similar Logseq feel in Obsidian, here are some that might help:

- Outline
- Outliner (separate to above)
- Zoom
- Backlinks
- Outgoing links
- Strange New Worlds

---

***Disclaimer:**
This post was written with the help of a number of tools that use AI. First, I added my original YouTube video to Readwise's Reader application. Readwise generates a transcript from this video, which I then export to a Markdown file. I process the text in Quillbot's online tool to paraphrase and remove some of the parsing errors I get from Readwise. I then ask ChatGPT to summarise my thoughts, which I then use as the starting point for this post. It still takes a lot of effort (over a day this case!) to get it up to the standard that I'd like, but it's a great point of departure. The full video is available below.*
{{< youtube TW_UpX5Gk3E >}}

---

If you'd like to accelerate your personal knowledge management journey with Logseq, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button-one href="https://www.logseqmastery.com?utm_source=blog&utm_medium=post&utm_campaign=obsidian" >}}Take me to Logseq Mastery{{< /button-one >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button-two href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button-two >}}