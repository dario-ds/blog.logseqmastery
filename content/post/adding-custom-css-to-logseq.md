---
draft: false
title: "Adding custom CSS to your Logseq database"
date: 2023-02-27T15:36:00Z
description: "Custom CSS is a great way to make your database more visually pleasing. In this guide I break down a simple way to implement CSS in your database."
summary: "Custom CSS is a great way to make your database more visually pleasing. In this guide I break down a simple way to implement CSS in your database."
tags: ["CSS", "customisation"]
categories: ["How-to guides"]
cover:
    image: /CustomCSS.png
---

I was late on the uptake with custom CSS, but I have found it to be a valuable addition to my Logseq database. The visual cues make it more pleasant to interact with information, and the enjoyment of the experience should not be taken for granted in the PKM journey.

You can [find my custom CSS here.](https://github.com/dario-ds/logseq/blob/main/onestutteringmind.css)

## How to install custom CSS in Logseq

-   Copy the code from the Github page linked above
-   Open your _'Settings'_ menu in Logseq (this can be accessed using the shortcut 't s')
-   Click the _'Edit custom.css'_ button
-   Paste the code into the code editor
-   Voila!

## Some notes on my lack of CSS expertise

If you look through [this handy CSS reference](https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/CSS) you'll see that I'm not following best practices, but I'm satisfied with the outcome for my purposes.

The most important things to note when changing the appearance for a given element are identifying your target (i.e. the text that will trigger the different display of a page reference or tag), and adding the appropriate marker to indicate position.

**Tags:** .tag\[data-ref="target"\]{ }.content  
**Page references:** .page-reference\[data-ref="target"\]{ }.content  
**Data-ref patterns:** _(i.e. these will all work for the word target)_

-   \[data-ref="target"\] element whose target attribute value is exactly target
-   \[data-ref**^**\="tar"\] element whose target attribute value begins exactly with the string "tar"
-   \[data-ref**$**\="get"\] element whose target attribute value ends exactly with the string "get"
-   \[data-ref**\***\="rg"\] element whose target attribute value contains the substring "rg"

Now get out there and be an artist 😉

{{< rawhtml >}}
<iframe src="https://giphy.com/embed/11eSHfUlB284H6" width="480" height="406" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/haydiroket-painting-florida-11eSHfUlB284H6">via GIPHY</a></p>
{{< /rawhtml >}}
![](https://giphy.com/gifs/haydiroket-painting-florida-11eSHfUlB284H6)

---

If you found this post helpful, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button href="https://www.logseqmastery.com" >}}Take me to Logseq Mastery{{< /button >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button >}}