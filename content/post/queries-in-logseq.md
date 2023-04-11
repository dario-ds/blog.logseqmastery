---
title: "How to use queries in Logseq"
date: 2023-01-27T15:36:00Z
description: "Queries give users a powerful mechanism to retrieve information from their databases, and will take your usage of Logseq up a notch. This post is a collection of excerpts from Logseq Mastery."
summary: "Queries give users a powerful mechanism to retrieve information from their databases, and will take your usage of Logseq up a notch. This post is a collection of excerpts from Logseq Mastery."
tags: ["queries", "Boolean logic", "properties"]
categories: ["How-to guides"]
cover:
    image: QueryCover.png
---

## What are queries?

A query is a way to **ask your database questions.** You can use queries to search for backlinks (and tags - these are interchangeable in Logseq), blocks with user-defined properties, text snippets, date-based information and different management task statuses and priorities. Queries are particularly useful when looking for a combination of information, as you can use Boolean operators to refine your results. They can be **thought of as saved searches.** The "questions" remain as a block in your database, which means you can return to the query when you need to ask the same questions.

## Why use queries at all?

Queries are useful for building dashboards for your most repeatable workflows, for example, project and task management dashboards. They also create accessible searches when you require ease of reference in a particular location in your database. Queries are the easiest way to find text quickly in your database, rather than using 'Unlinked references'. Finally, they are a great tool for building indexes of information, particularly when you have used properties consistently in your database.

## What is returned by a query?

**Queries return a subset of blocks that match your input criteria**. Looking at the simplest example of a _[[backlink]]_, a query will return the following:

1. All blocks linked to _[[backlink]]_ (i.e. _[[backlink]]_ appears in the block)
2. All blocks indented below a block linked to _[[backlink]]_
3. All blocks on the _[[backlink]]_ page

## How to use queries in Logseq

The standard way of bringing up a query is using the _/_ command to bring up the context menu. Then type _query_. It will automatically input the standard query format _{{query }}_. You can then enter a number of parameters to refine what is returned by your query.

- **User-defined properties:** _{{query (property property_name property_value) }}_
  - _property_name_ is the property that you have defined. My typical examples are _type::, producer::_, etc.
  - _property_value_ is optional. You can use normal text or _[[backlinks]]_
- **Text snippets:** _{{query "search text in quotation marks"}}_
- **Date-based information:** _{{query (between start end)}}_
  - _start_ and _end_ can be either dates from the journal, e.g. _[[Jan 1st, 2023]]_, natural language, e.g. _yesterday_ or the built-in operators _**+**_ and **-** with time frames _min_ for minutes, _h_ for hours, _d_ for days, _w_ for weeks, _m_ for months and _y_ for years
- **Task statuses:** _{{query (task task_status)}}_
  - _task_status_ can be _later_, _todo_, _now_, _doing_, _waiting_, _cancelled_ or _done_.
- **Priorities:** _{{query (priority priority_level)}}_
  - _priority_level_ can be either _A_, _B_, or _C_.

## How does Boolean logic work?

The image below is taken from Logseq Mastery where there is a full video dedicated to this topic. However, the [second video](https://youtu.be/qQ8DzumRZkM) linked below also explains this diagram in detail.

![](/BooleanLogic.png)

## Helpful tips when working with queries

-   Include a user-friendly description of what you are trying to query in a block above your actual query. You can then indent the main query under that high-level block. This is like building documentation into your database and helps you remember what you were trying to do.
-   Text queries are particularly valuable when searching for information in your database that you haven't linked to, rather than using Unlinked References. Note that text queries are case sensitive.
-   Avoid queries that will return too many blocks, as this will slow down Logseq's performance.
-   When you have a query, it returns a long list of all the blocks. It is often helpful to pivot those results into a table for easy readability. This feature becomes particularly powerful if you've used properties consistently.

---

### This post is a compendium to my videos on YouTube which all look at how to use queries in Logseq:


{{< youtube bg_NpHkecdY >}}

---

{{< youtube qQ8DzumRZkM >}}

---

{{< youtube GDauxjx_bdA >}}

---

If you found this post helpful, you might enjoy the full Logseq Mastery course. The course has a wealth of videos, detailed write-ups and diagrams to quickly master Logseq and save you plenty of time and headaches.

{{< button href="https://www.logseqmastery.com" >}}Take me to Logseq Mastery{{< /button >}}
{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    Want to browse the course outline first? Click on the button below to see the user guide for Logseq Mastery and to view the latest updates.
  </p>
{{< /rawhtml >}}


{{< button href="https://updates.logseqmastery.com" >}}Logseq Mastery user guide and updates{{< /button >}}