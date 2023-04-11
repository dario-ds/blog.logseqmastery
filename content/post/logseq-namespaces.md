---
title: "How to use namespaces in Logseq"
date: 2022-11-30T15:36:00Z
description: "Namespaces are a helpful feature in Logseq for those who like top-down approaches to information management. This post is a collection of excerpts from Logseq Mastery"
summary: "Namespaces are a helpful feature in Logseq for those who like top-down approaches to information management. This post is a collection of excerpts from Logseq Mastery."
tags: ["namespaces", "organisation", ""]
categories: ["How-to guides"]
cover:
    image: Namespace.png

---

## What are namespaces?

Namespaces are a helpful feature in Logseq for those who like top-down approaches to information management. Namespaces are characters that **allow for the addition of hierarchy in a file system.** Suppose you think of a hierarchical folder structure in Windows Explorer. If you navigate to a particular folder and then click on the folder 'breadcrumbs', you'll see something like this: _'C:\Users\YourName\Downloads'_ . In this example, the namespace character is a backslash _'\'_ and it indicates a branch of a higher root folder.

## How are namespaces implemented in Logseq?

In Logseq, namespaces are a **special type of page that allow for hierarchy in the page names.** The namespaces character in Logseq is a forward slash, _'/'._

By way of example, I would like to take notes on different Brazilian Jiu-Jitsu (BJJ) related information and add some hierarchy to my notes. Hypothetically I learn about a new choke, the 'triangle'. I could then create a page _-__**-BJJ/chokes/triangle]].**_ If I try a new gym, I might want to keep track of all the people that I meet there, so I create a page _**--BJJ/gyms/Renzo Gracie Cape Town]].**_ Logseq will create a Markdown file for each new namespace page you create. In the actual file name, the _'/'_ is replaced by _'%2'._ So the files created above would be _**BJJ%2chokes%2triangle.md**_ and _**BJJ%2gyms%2Renzo Gracie Cape Town.md**_

Whilst namespaces do create hierarchy in your database, the implementation differs slightly from traditional folders. It's important to remember that all pages serve as nodes in your database. Namespaces can therefore perform two functions:

1. Namespace pages can **store information.**
2. Namespaces can be used as a node by which to **create links to blocks in your database for easier retrieval.**

So if I meet someone new in the gym, Marcelo Garcia (I wish...), I could enter that information in one of two ways. I can enter a block on my daily journal and link that block to the gym (see below), or I could navigate to the page and enter Marcelo Garcia as an actual block on that page.

- Marcelo Garcia --BJJ/gyms/Renzo Gracie Cape Town]]

## The utility of namespaces

Namespaces' are particularly useful in retrieving information. They provide you with access to a new panel below your Linked References to navigate namespaces. Howeveryou can also **create namespace queries to generate automatically updating indices for your content**. This is my preferred approach.

For example, I could generate a list of all my BJJ-related content with the query **{{namespace BJJ}}**. The output from my personal database appears as below, which enables me to easily navigate all the BJJ-related content in my database.

![](https://d1yei2z3i6k35z.cloudfront.net/1932909/63875fc7dac9c_Capture.PNG)

When you first use Logseq it might be tempting to use namespaces for everything. This can lead to headaches later on, however, as imposing a rigid top-down structure from the beginning limits your flexibility. **I'd encourage you to delay your use of namespaces until you have refined your understanding of how they might suit your workflows.**

---

If you found this post helpful, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button href="https://www.logseqmastery.com" >}}Take me to Logseq Mastery{{< /button >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button >}}