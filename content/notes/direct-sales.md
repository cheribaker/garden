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

It's also worth noting that Shopify frequently updates their themes, so if you've written custom code anywhere on the site when you move to a new version of the theme, you'll need to check for compatibility with your changes. Hence, it's probably smart to have a "light touch" when modifying the theme iself.

We briefly considered Gumroad, E-Junkie, and Payhip for our store, but they didn't offer all the features we wanted.

## Features
I'm particularly happy about these features on our web store:
- An attractive, clean interface.
- A "reading order" page that updates dynamically to show my books in the correct reading order.
- Multi-retailer links on every book page.
- Collections pages for each series. (like [this one](https://www.cheribaker.com/Ellie))
- Integration with my mailing list software (MailerLite) so I can see what works and what doesn't for sending traffic to the site.
- Integration with MailerLite also allows me to "add a product" from my store directly into a newsletter as a block element. That's handy!

Multi-retailer links and the reading order page (and many other small tweaks) were hand-coded by my partner in crime, Patrick. He does good work! Our site is a lightly modified version of Shopify's "Dawn" theme. 

## Revisions Since Launch

- We added "Add to Cart" buttons on the front page. Initially we liked the clean look of only showing the book covers, but this meant a *lot* of clicking for anyone who wanted to add multiple products to a cart quickly.

## Problems & Solutions

#### Tax compliance
Tax compliance is a pain in the ass because every location has its own rules and paperwork. Some countries make it easy; you simply don't report anything until you make a certain amount of money in that country. Others require up front registration and continual tax filings even when you make zero money there.

We currently sell to six markets where I have the most readers:
* USA
* Canada
* UK 
* EU 
* Australia
* New Zealand

EU tax compliance is difficult because they have a lot of regulatory hoops to jump through, including registration with an intermediary located in the EU. We use a service called *EAS EU & UK Compliance* that integrates with Shopify. We've also had to register for a UK Vat number, a process that took about four months, and which requires regular tax filings regardless of income.

**Transaction Costs**: Because selling a book to customers in the EU results in a per-transaction compliance cost of 1.25 EU, functionally this means I can't sell any book for less than $2.99 in my store. A 99c short story could end up costing me money with every sale, for example.

#### Policies
A store is required to have things like a clearly articulated return policy, terms of service, a privacy policy, and a physical address and phone number. Researching our policies and so forth took a while, so I'd recommend starting that process sooner rather than later if you're setting up a store. You may also want an attorney to look over your docs.

#### Multi-Retailer Links
While I would obviously be thrilled if every reader chose to buy books from me directly, it's important that readers have a choice. We handled this by adding a "retailer links" section below the buy-buttons on our webstore. It may seem counterintuitive to direct customers AWAY from your store, but this works great because:

- Instead of providing 5-10 different links in every newsletter I send, I can include just one - the one that goes to my store.
- With every click, readers are reminded that they can buy from me directly (although it's not required)
- A single canonical link for each book means I'm always sending traffic to my own website.
- It makes it easy for readers to find the store they want.

*note: Patrick coded this addition for us*

#### Reader Education
People may be nervous about inputting their credit card into a website they don't know. They may also be nervous about buying a book directly from a website, especially if they're used to using a particular store app.  I've added a FAQ and some language to explain things, but this will likely be a hurdle to overcome.

#### Payment Processors
We've set up standard credit card processing, Shopify Payments (Shop Pay), Google Pay, and Apple Pay. It appears that Apple Pay works great on iOS devices but it requires using the Safari browser.

I was tempted to add Paypal as a payment option, because they're popular, but I've read too many stories about small businesses being screwed over by Paypal without recourse.

#### Links in End Matter

Some book retailers get salty if you include end-matter links that go to other retailers. While I understand this, to a degree, I wasn't going to build a separate edition of each e-book for each retailer as at a certain point that becomes stupidly complicated.

We use generic "Collection" pages for each series with a simple forwarding URL like:

`` www.cheribaker.com/Ellie ``

Thus readers are redirected to a "series landing page" that I control, and when they click a book cover, they can find the whole list of retailer links for that book, including the "add to cart" button for purchasing from me.

#### RSS on Shopify

Shopify allows you to set up one or more "blogs" on your website, and I've set up two, one for essays and one for travel writing, although they are less blogs than they are places for me to store longer-form pieces to share within my newsletter.

I had a hard time finding the RSS feeds. The current correct format is:

`` http://your-website.com/blogs/blog-name.atom ``

I don't see any blog export feature on Shopify, so it's important to keep complete copies of your posts, images, and URLs offline in case you need to regenerate your blog and links on another service in the future.

#### Cookies and Privacy

Shopify comes loaded with default settings that probably increase sales, but which I personally don't approve of. Things like tracking cookies and emails to people to remind them to finish their 'abandoned cart.'' Also, they offer a 'pay in installments' option for financing.  I turned off as much of this stuff as I was able to, but the site is still a bit nosier than I'd prefer. 

#### International Pricing

Shopify will auto-convert US prices for the market currencies we support. However, there are limitiations. The standard version of Shopify doesn't support custom international prices, so I can neither "round up/down" to the nearest .49 or .99, nor can I adjust international prices to be a better match for cost-of-living parity.

Unless you spend a LOT of money for the super fancy version of Shopify, you're stuck with their standard conversion, and no customization.

#### Reviews/Social Proof

It's possible to set up reviews for products in your store. To be frank, book reviews I saw on other author stores read like cherry-picked reviews from their friends and biggest supporters, and I didn't want the headache of dealing with review moderation on my site. For now, I've elected not to bother soliciting reviews on my own site.

## Stuff for the Future

We're looking into selling audiobooks and paperback books through our store. Lulu offers paperback drop-ship integration, and Bookfunnel would work for audiobook delivery. Before we add more complexity, we want to get a handle on our new e-book store and learn how to sell books there.

To my fellow booksellers, I hope this helps! Cheers.