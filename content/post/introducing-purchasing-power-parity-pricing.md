---
title: "Introducing purchasing power parity pricing to Logseq Mastery"
date: 2023-04-26T10:36:00Z
draft: false
description: "Logseq Mastery now has purchasing power parity (PPP) pricing to make the course more accessible to a global audience."
summary: "Logseq Mastery now has purchasing power parity (PPP) pricing to make the course more accessible to a global audience." 
tags: ["PPP"]
categories: ["Thought pieces"]
cover:
    image: "/ppp.png"
---

### Introduction

My aim with Logseq Mastery is to make the knowledge available to as wide an audience as possible. I've tried to account for this in my pricing, keeping prices low so that cost doesn't become the main obstacle. Nevertheless, a 'one-size-fits-all' approach to pricing isn't feasible in a global economy, which is why I've decided to implement purchasing power parity (PPP) pricing for Logseq Mastery.

### How PPP pricing work?

Purchasing power parity (PPP) pricing is an economic concept that considers the purchasing power of currencies in their local countries, rather than relying solely on market exchange rates. Economists use price data to compare the cost of goods and services in each country, and then normalise them based on a single currency exchange rate, typically the US dollar. The relative purchasing power of each currency is then determined by comparing this normalised cost across countries.

One index which has become popular is the [Big Mac Index, developed by The Economist](https://www.economist.com/big-mac-index). The index works by converting a country's local Big Mac price into US dollars to determine if a currency is over- or under-valued. The pricing discrepancy also reveals the relative PPP.

For example, taking my home country, South Africa, and using the July 2022 dataset, the price for a Big Mac is R39.90. This equates to $2.34, applying the exchange rate at the time of R17.04/ $. In the US, a Big Mac costs $5.15. This implies that the South Africa Rand has 45% purchasing power of the US dollar (2.34/5.15), and that prices should be reduced to take account for that.

The Big Mac Index is obviously a simplified way of analysing currency values, as it doesn't account for differences in production costs, taxes, and other factors impacting Big Mac prices globally. Even so, it serves as a useful benchmark for simple applications.

### How do I plan to implement it?

There is an excellent SaaS called [Parity Deals](https://www.paritydeals.com/) that integrates with course hosting platforms and offers users a discount banner based on their IP address. Of course, all of this comes with an ongoing cost at a time that I'm trying to limit my number of SaaS subscriptions. 

So, inspired by [Marie Poulin](https://notionmastery.notion.site/Notion-Mastery-Parity-Pricing-c7b61b316de941fd954a7e4902fef181), I've chose to experiment with my own version for a few months, which gives me the added benefit of seeing how the discounts are applied. I combined the [World Bank's PPP dataset](https://data.worldbank.org/indicator/PA.NUS.PPPC.RF) and the Economist's Big Mac index to create a database of different countries and their discount eligibility. Users can register for a discount via an Airtable form, and upon approval will receive an email with the discount code and a link to a special landing page.

This is a trial solution, and I welcome user feedback. I may end up defaulting to Parity Deals in the future.

### An appeal for good faith

While the ParityDeals.com service might be vulnerable to IP spoofing, I'm susceptible to dishonesty from people in high-income countries who possess passports or documentation from low-income countries. I've already had an instance of this, which I only discovered because the person specifically asked me if they could trial the approach, but then added the country where they're currently residing in the sign-out form. While there may have been other reasons behind this, it was nonetheless disheartening. As I navigate this new pricing structure, I kindly ask potential users to respect the purpose behind PPP pricing and act in good faith.

### Conclusion

I hope that implementing PPP pricing for Logseq Mastery will make the course more accessible, and look forward to including a more global audience in the course. While the current trial solution has its limitations, I will be improving the process based on user feedback, so please reach out if you have any feedback.

{{< button-two href="/ppp-pricing-eligibility" >}}View PPP pricing eligibility{{< /button-two >}}
{{< rawhtml >}}<br>{{< /rawhtml >}}
{{< button-one href="https://airtable.com/shrkgXimQP3GJUNKT" >}}Register for a PPP discount{{< /button-one >}}

