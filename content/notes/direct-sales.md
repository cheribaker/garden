---
title: "Setting up an Author E-commerce Site"
tags:
- projects
weight: 0
---

*Notes on a project in process.*

### Status
We're developing the first version of our store, which will sell e-books only. In the near future, we'll add paperback sales.

### Goals
- To reduce dependence on e-commerce platforms like Amazon.
- To increase royalties per sale.
- To provide better customer service to our readers.
- To retain control over key business decisions.

## Limitations
- We use Bookfunnel for ebook distribution, so we needed to select e-commerce tools that are compatible with Bookfunnel webhooks.
- We use Mailerlite for customer communications, ideally our store will be compatible so we don't need to manually import customers between systems.

## Tech Stack (1.0)
- Shopify  (Store, Cart, & Payment Processing)
- Bookfunnel (eBook delivery & multi-device customer support)
- Lulu Express (Print on Demand)
- Mailerlite  (Customer Communications)

## Tricky Bits

#### Tax compliance
It gets a bit complicated! We'll start by selling to these markets.
* USA
* Canada
* UK
* EU
* Australia
* New Zealand

#### KU vs Non-KU Books
A few of my series are exclusive to Amazon (for the time being), so P coded us a nice redirect that auto-sends shoppers to the correct place.

#### Reader Education
I wrote a FAQ to demystify the process of getting an ebook onto a reader's device of choice.

#### Payment Processors
We've set up standard credit card processing, Shopify Payments (Shop Pay), Google Pay, and Apple Pay. I was tempted to add Paypal but the sheer number of "they fucked us sideways" stories from small businesses scared me off Paypal for now.

## Current Priorities

We're wrapping up our last few work items and preparing for site migration.

