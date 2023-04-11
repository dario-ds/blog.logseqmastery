---
title: "How I use Omnivore in my read-it-later workflow for articles"
date: 2022-12-16T10:00:00Z
description: "Discover Omnivore, the read-it-later app that organises online content and integrates seamlessly with Logseq."
summary: "Discover Omnivore, the read-it-later app that organises online content and integrates seamlessly with Logseq."
tags: ["read-it-later", "Omnivore"]
categories: ["How-to guides"]
cover:
    image: Omnivore.png

---

## What is Omnivore?

Omnivore is an open-source read-it-later application that allows users to save and organise online content (e.g., tweets, articles, and blog posts) for later reading and reference.

Lots of folks use ReadWise's Reader app as their preferred read-it-later app. It is a great product, which I still use for some workflows (see disclaimer below). But there was one pain point that made me look for another solution. Reader can only export your highlights and annotations as pages and not as blocks. This does not work for my reading workflow or for the way that I manage information in my database.

In my database, notes on articles, videos, podcasts, and tweets are small chunks of information that don't deserve to be elevated to pages. The proliferation of pages that result from Readwise imports was not to my liking. Having too many pages can also impact Logseq's performance, even though it has improved dramatically recently. I knew this was something that I wanted to avoid, and for some time I had some hacky workarounds with Reader, exporting to Markdown and painfully copy-pasting into Logseq. However, I found myself avoiding this workflow—even avoiding reading in Reader—because I knew the frustration that was coming later.

And then I found Omnivore.

Or rather, Omnivore found me. The Omnivore team actually reached out to me to tell me about the app the day after I was onboarded onto Reader as a beta user. I don't like changing applications at the drop of a hat, so I wanted to give Reader a proper go, and I politely declined the invitation to try out Omnivore. 

A few months later, the team reached out to me again to see if there was anything they could learn from my Readwise workflow. We scheduled a call, and this time I saw the app working firsthand. I saw how Omnivore worked with the same paradigm of content as blocks, and it was clear that my reading and processing workflow would work perfectly in Omnivore without the hacks of Reader.

Omnivore is mobile-friendly, a non-negotiable in this space, with both iOS and Android apps. (I prefer to use the progressive web app because the official application defaults to dark mode, and I prefer reading dark text on a light background.) The user interface is minimal and appealing.
The ability to create an email alias that lets you subscribe to online publications is also a basic requirement in read-it-later apps, and setting this up in Omnivore is simple. 

Since I started using Omnivore, I've found myself reading more and retaining more information. The seamless integration with Logseq is a major benefit, and the team has been great to interact with, which is always a plus. If you're someone who takes a lot of notes as you read, I recommend giving Omnivore a try. It's become an integral part of my workflow, and I'm confident it will be for you too.

## Integrating Logseq and Omnivore

[Brian Sunter](https://twitter.com/Bsunter) has written a handy guide to [getting started with Omnivore here](https://briansunter.com/pages/omnivore-logseq-guide), but I'll break down the basics below.

- You first need to create an Omnivore account [via their website](https://omnivore.app/). I also recommend that you install the browser extension. Here is the [link to the Chrome browser extension.](https://chrome.google.com/webstore/detail/omnivore/blkggjdmcfjdbmmmlfcpplkchpeaiiab?hl=en-GB)
- Install the Omnivore plugin in the Logseq marketplace, then navigate to your plugin settings.
  - Three dot menu at top right of screen -> "Settings" -> "Plugins" on left panel -> Select "Omnivore"
- Go back to your Omnivore web app and create an API key by clicking on your user profile at the top right of your screen, and selecting "API keys"
- Copy this API key and paste it into your settings in the relevant box in your Omnivore plugin settings in Logseq.
- Once you've added some articles, you can then activate the Omnivore import by clicking the plugin icon at the top of your screen.

## My basic workflow for using Omnivore

- Save all sources to Omnivore wep-app
  - Omnivore has a simple browser plugin that allows you to add articles at the click of a button or by using shortcut **"Alt + O"**
  - You can submit tweets to Omnivore by using the iOS or Android apps and using the "Share Tweet via" context menu.
- I do most of my reading on my tablet and make highlights and annotations about what I've read as I go along.
- If once I've finished reading a source, I decide I want to send it to Logseq, I add my custom label "Sent to Logseq" and then I archive the source using the standard **"e"** shortcut. (Note: this works for Reader, Gmail, and many other programmes.) If I haven't highlighted anything or taken any notes, I simply archive the source.
- When I want to import my Omnivore notes into Logseq, I click the Omnivore Plugin button in Logseq, which imports all the articles that I've labelled "Sent to Logseq" to a page in my database called "Omnivore imports".
  - I've setup a custom filter in my Omnivore plugin settings by changing the filter to "advanced" and then only importing those articles that have the label “Sent to Logseq”. I do this to avoid all the articles syncing to Logseq, even if I hadn't read them.
- When I want to process an article in my database, I move that article to the journal page for the current day. I then clean up my notes and add tags to the parent-level block that will help me find the article again.
  - If I needed to tag something that the tag in the parent-level block didn't cover, I would tag blocks at the individual level.

## Why do I follow this approach?

This approach helps me keep track of what I've processed. I treat it like a Kanban board for reading, where the three columns are as follows:

- synced to be read later -> read and annotated -> processed in my database.

I've also configured my import settings to enable me to distinguish between what is others' writing (i.e. highlights) and what are my notes. Highlights are turned into a Markdown quotation block by adding a **">"** in front of the block. My notes on the block are then indented underneath the highlighted snippet, although I often remove the original highlight and just leave my own notes.

All my templates are shared below so that you can implement this workflow if it sounds good to you.

---

## My Omnivore plugin settings

![](/Omnivore1.png)
![](/Omnivore2.png)

**Note that I created the "Sent to Logseq" label in the Omnivore interface.** I only add the label to articles that I want to send to Logseq.

Also note that the implementation of the advanced filter has also changed since I released the video.

Now, instead of this format in the advanced filter box... 
    
    label:\"Sent to Logseq\"

you should use this format:
    
    label:"Sent to Logseq"

## Article template text:

    ### {{{title}}}
    collapsed:: true
    {{#author}}
    producer:: [[{{{author}}}]]
    {{/author}}
    input:: [[articles]]
    link:: {{{originalUrl}}}
    source:: [[Omnivore imports]]
    tags::

---

### Here is the full YouTube video for reference:

{{< youtube Cc6DbBtOs14 >}}

---

*Disclaimer:*
This post was written with the help of a number of tools that use AI. First, I added my original YouTube video to Readwise's Reader application. Readwise generates a transcript from this video, which I then export to a Markdown file. I process the text in Quillbot's online tool to paraphrase and remove some of the parsing errors I get from Readwise. I then ask ChatGPT to summarise my thoughts, which I then use as the starting point for this post. It still takes a lot of effort to get it up to the standard that I'd like, but it's a great point of departure.

---

If you found this post helpful, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button-one href="https://www.logseqmastery.com" >}}Take me to Logseq Mastery{{< /button-one >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button-two href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button-two >}}