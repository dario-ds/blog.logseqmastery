---
draft: false
title: "Adding custom CSS to your Logseq database"
date: 2023-02-27T15:36:00Z
description: "Custom CSS is a great way to make your database more visually appealing. In this post I break down a simple way to implement CSS in your database."
summary: "Custom CSS is a great way to make your database more visually appealing. In this post I break down a simple way to implement CSS in your database."
tags: ["CSS", "customisation"]
categories: ["How-to guides"]
cover:
    image: /CustomCSS.png
---

## Introduction and quick start

I recently discovered the power of custom CSS in Logseq and have found it to be an invaluable addition to my database. The visual changes not only make it more aesthetically pleasing, but also provide subtle cues that encourage interaction with the information in your database. 

I've shared [my custom CSS here](https://github.com/dario-ds/logseq/blob/main/onestutteringmind.css) as a quick start reference. To install this CSS, follow these steps:

-   Copy the code from the GitHub page linked above
-   Open your _'Settings'_ menu in Logseq (this can be accessed using the shortcut 't s')
-   Click the _'Edit custom.css'_ button
-   Paste the code into the code editor
-   Voilà, you're all set!

For those interested in making updates to the CSS, I'll delve into more detail below, as it's useful to understand what you're working with.

## A (slightly) deeper dive into CSS

### Identifying CSS elements (selectors)

The first step is know the type of element you want to modify in Logseq. In this post, we'll examine two simple elements: #tags and [[page references]].

To update the appearance of #tags, use the following:
    
    .tag{

      }.content  
  
To update the appearance of [[page references]], use the following:
    
    .page-reference{

     }.content  

### Specifying text

You can further refine the elements that you want to change by specifying text in the [data-ref] parameter.

If you have a tag, #target, or page reference, [[target]], you would use the following code:

    .tag[data-ref="target"]{

      }.content  

and

    .page-reference[data-ref="target"]{

     }.content  

### Identifying patterns of text

You can also define different positions of target text in the [data-ref] parameter. In the examples below, we will look at some patterns which will work for the word "target":

To target an element that **begins with specific characters**, use the ^ sign. For example, if the element value is "target", use:

    [data-ref^="tar"]

To target an element that **ends with specific characters**, use the $ sign. For example, if the element value is "target", use:

    [data-ref$="get"]

To target an element that **contains a substring of certain characters**, use the * sign. For example, if the element value is "target", use:

    [data-ref*="rg"]

### Using different CSS properties

CSS allows you to alter the visual appearance by modifying different properties, such as colours, spacing and font-size. Some common properties are listed below, but if you're looking for a comprehensive guide, [the Mozilla Developer Network (MDN) Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#index) is the place to go. 

    { color:; 
      background-color: 
      padding: ; 
      border-radius:; 
      margin:; 
      font-weight;
      }.content

### Adhering to CSS best practices

If you refer to this [this handy CSS reference, also from the Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/CSS), you'll notice that my approach doesn't follow best practices. I've condensed all my CSS parameters onto a single line, rather than using multiple lines. However, I'm satisfied with the outcome for my purposes, and it simplifies editing my work.

Best practice would suggest that instead of this:

      a.tag[data-ref="target"]{ padding:0 7px; border-radius:7px; margin:2px 0; color:white !important; background-color:grey}.content

I should use this 

      a.tag[data-ref="target"]{ 
        padding:0 7px; 
        border-radius:7px; 
        margin:2px 0; 
        color:white !important; 
        background-color:grey
        }.content

## Conclusion

Visual enhancements to your personal knowledge management tool of choice should not be taken for granted. If it improves your experience, it will likely improve your utilisation of the tool too. Now it's your turn to experiment with custom CSS and unleash your inner artist in your Logseq database. Happy customising!

---

If you found this post helpful, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button-one href="https://www.logseqmastery.com?utm_source=blog&utm_medium=post&utm_campaign=css" >}}Take me to Logseq Mastery{{< /button-one >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button-two href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button-two >}}