## Local Setup

```
bundle install
bundle exec jekyll s
```

## Images
Images are located in `/assets/img/` folder and it's subfolders.

## Pages
Page content (images, text, buttons) can be edited in the front matter of page markdown files, e.g. `about-fio.md` (located in the root):


```
---
layout: about
title: About FIO

feature:
  heading: The Foundation
  image: /assets/img/about-fio/FIO-ISO.svg
  description: |
    The Foundation for Interwallet Operability is a industry consortia, consisting of leading wallets, exchanges, crypto payment processors, and various other entities and community members dedicated to the pursuit of blockchain usability through the FIO Protocol.

  button:
    text: Learn more about FIO
    url: https://kb.fioprotocol.io/foundation/foundation-overview

---
```

Descriptions accept [markdown syntax](https://docs.github.com/en/free-pro-team@latest/github/writing-on-github/basic-writing-and-formatting-syntax).

## Favicon
Favicon image setting is located in `_config.yml`:

```
favicon:                  /assets/img/favicon.ico
```


## Google tag
Google tag ID can be set in `_config.yml`:
```
google_analytics:         GTM-WWSZ8NR
```

## Callout (Mailchimp signup) section
Callout setting are located in `_config.yml`:

```
mailchimp:
  form_action:            https://foundation.us19.list-manage.com/subscribe/post?u=83e722420b22435be258e8ea5&amp;id=0849d2c011
  hidden_name:            b_83e722420b22435be258e8ea5_0849d2c011

social_networks:
  telegram:               https://t.me/joinFIO
  discord:                https://discord.gg/pHBmJCc
  facebook:               https://www.facebook.com/officialFIO
  reddit:                 https://www.reddit.com/r/officialFIO
  linkedin:               https://www.linkedin.com/company/officialfio/
  twitter:                https://twitter.com/joinFIO

callout:
  heading:                Keep in Touch
  description:            Sign up for our monthly newsletter and join us on social!
  placeholder:            Enter Email Address
```

## Header navigation

Header navigation link settings are located in `_data/navbar.yml`.

## Footer

Footer column link settings are located in `_data/footer.yml`.

Footer bottom bar settings are located in `_config.yml`:

```
footer:
  copyright:              "&copy; 2020 FIO"
  link:
    title:                Privacy Policy
    url:                  /privacy-policy/
```

## Ecosystem data

Ecosystem data can edited in `_data/ecosystem.yml`:

```
- category: Wallets
  items:
  - heading: Edge
    featured: true
    featured_addresses: true
    status: integrated
    image: /assets/img/ecosystem/edge.png
    url: https://edge.app/
    list:
    - FIO Token
    - Send to FIO Address
    - Receive to FIO address

  - heading: Edge
    featured_addresses: true
    status: integrating
    image: /assets/img/ecosystem/edge.png
    url: https://edge.app/
    list:
    - FIO Request
    - FIO Domains
    - FIO Data
    
- category: Exchanges
  items:
  - heading: Some other
    featured: true
    image: /assets/img/ecosystem/edge.png
    url: https://edge.app/
    list:
    - Send to FIO Address
    - Receive to FIO address
    - FIO Data
```
Items are nested into categories. 

Adding `featured: true` to an item will display it in "The FIO Ecosystem" section on home page. Status options are: `integrated`, `integrating`, `preintegration` or leave blank for default.

Adding `featured_addresses: true` to an item will display it on the  "Free FIO Address".

## Ecosystem data

Ecosystem data can edited in `_data/ecosystem.yml`:

```
- title: Fourth featured news are many variations of passages of Lorem Ipsum available
  featured: true
  featured_news: true
  image: https://via.placeholder.com/600x120
  url: https://edge.app/
  publication: Lorem
  date: 10/02/2018

- title: Fith are many variations of passages of Lorem Ipsum available
  image: https://via.placeholder.com/600x120
  url: https://edge.app/
  publication: Lorem
  date: 10/02/2018
```

Adding `featured: true` to an item will display it in "Featured Press" section on Press page. 

To feature and item in "News and Events" section on homepage add one of the folowing to an item:

- `featured_blog: true`
- `featured_media: true`
- `featured_news: true`