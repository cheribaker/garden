---
title: "Setting up an E-Commerce Bookstore"
tags:
- projects
weight: 0
---

Notes and lessons learned on setting up an e-commerce site to sell e-books directly. This project was a two-person effort. I (Cheri) did most of the design work and Patrick did the coding and customization.

### Status
Site is [Live](http://www.cheribaker.com).

### Goals
- To reduce dependence on third-party e-commerce platforms like Amazon.
- To increase royalties per sale.
- To provide better customer service to our readers.
- To retain control over key business decisions.
- To make DRM-free ebooks available for customers who prefer them.

## Limitations
- We use Bookfunnel for ebook distribution, so we needed to select e-commerce tools that are compatible with Bookfunnel webhooks.
- We use Mailerlite for customer communications, ideally our store will be compatible so we don't need to manually import customers between systems.

## Technology
- Shopify  (Store, Cart, & Secure Payment Processing)
- Bookfunnel (eBook delivery & multi-device customer support)
- Mailerlite  (Customer Communications)

Shopify is great because it's powerful in the things that matter (secure payment processing, reporting) and because it integrates with a lot of services we use (Bookfunnel, MailerLite) but it also sucks at times because features which would seem very basic are sometimes missing. They offer many features as "plug ins" but almost every plugin comes with a monthly fee.

We briefly considered Gumroad, E-Junkie, and Payhip for our store, but they didn't offer all the features we wanted.

## Features
I'm particularly happy about these features on our web store:
- An attractive, clean interface.
- A "reading order" page that updates dynamically to show my books in the correct reading order.
- Multi-retailer links on every book page.
- Collections pages for each series. (like [this one](https://www.cheribaker.com/Ellie))
- Integration with my mailing list software (MailerLite) so I can see what works and what doesn't for sending traffic to the site.

Multi-retailer links and the reading order page (and many other small tweaks) were hand-coded by my partner in crime, Patrick. He does good work! Our site is a lightly modified version of Shopify's "Dawn" theme. 

## Problems & Solutions

#### Tax compliance
Tax compliance is a major pain in the ass because every location has its own rules and paperwork. Some countries make it easy, you simply don't report anything until you make a certain amount of money in that country. Others require up front registration and continual tax filings even when you make zero money there.

We currently sell to six countries where I have the most readers:
* USA
* Canada
* UK 
* EU 
* Australia
* New Zealand

EU tax compliance is difficult because they have a lot of regulatory hoops to jump through, including registration with an intermediary located in the EU. We use a service called *EAS EU & UK Compliance* that integrates with Shopify. We've also had to register for a UK Vat number, a process that took about four months, and which requires regular tax filings.

**Transaction Costs**: Because selling a book to customers in the EU results in a per-transaction compliance cost of 1.25 EU, functionally this means I can't sell any book for less than $2.99 in my store. A 99c short story could end up costing me money with every sale, for example.

#### Multi-Retailer Links
While I would obviously be thrilled if every reader chose to buy books from me directly, it's important that readers have a choice. We handled this by adding a "retailer links" section below the buy-buttons on our webstore. It may seem counterintuitive to direct customers AWAY from your store, but this works great because:

- Instead of providing 5-10 different links in every newsletter I send, I can include just one - the one that goes to my store.
- With every click, readers are reminded that they can by from me directly (although it's not required)
- A single canonical link for each book means I'm always sending traffic to my own website.
- It makes it easy for readers to find the store they want. And I do want them to have a good experience, no matter where they shop.

#### Reader Education
People may be nervous about inputting their credit card into a website they don't know. They may also be nervous about buying a book directly from a website, especially if they're used to using a particular store app.  I've added a FAQ and some language to explain things, but this will likely be a hurdle to overcome.

#### Payment Processors
We've set up standard credit card processing, Shopify Payments (Shop Pay), Google Pay, and Apple Pay. It appears that Apple Pay works great on iOS devices but it requires using the Safari browser.

I was tempted to add Paypal as a payment option, because they're popular, but I've read too many stories about small businesses being screwed over by Paypal without recourse.

## Stuff for the Future

We're looking into selling audiobooks and paperback books through our store, but not immediately.  I'm also looking into "quick add" buttons for the front page, to minimize clicking needed when adding multiple books to a cart.