---
layout: post
title: Project ideas
---

* make-your-own-smoothie vending machine with dry ingredients
  * smoothie vending machines [exist](https://trendi.com/the-smoothie-machine/) (maybe not with dry ingredients) 
* japanese-style vending machines in North America that sell food like burgers
* android app that periodically deletes old files in Downloads folder
* postgresql code formatter that works
* manually-generated database of math techniques at a lower level than heuristics ("tricks")? e.g.
  * change the order of summation
  * break integral into sum of integrals on intervals and bound each integral
  * prove something about random variables by proving for simple RVs then proving
    for limit of sequence of simple RVs
  * take pairs of adjacent terms in a sum and simplify their sum then add them up
  * replace a-b with (a-x)+(x-b)
  * rationalize the denominator
  * etc.

  the value depends on how easy it is to search (e.g. tags?), how much
  work it takes to build the database, how likely new problems are to be
  solved by past tricks vs. new tricks, whether people would already have
  memorized common tricks, etc.
* vim plugin that renders latex math via [tex2utf](https://github.com/Pomax/tex2utf)
* shareable Instagram personality quizzes https://drive.google.com/open?id=1KAtYXXbS12hJ2POS00dZvH3TAaYIj3IgfJNKrtJr_jE
* people take photos of stuff and they're rewarded for accuracy and usefulness.
  * crowdsourced useful, local, current info
  * inspired by paying people to charge scooters
  * peer prediction or similar for usefulness ratings
  * people can browse on a map view
  * e.g. event here, sale at this store
  * time period of relevance is entered by the photo taker? or all photos last one day?
* web API security scanner with GPT
  * GPT sends requests attempting to uncover security by obscurity
  * GPT explores the website and gathers API calls or is given the API schema
  * ask it to come up with requests that might gain privileges, so it might add `?is_admin=1` for example. it would know the context and terminology of the API so if it's a site for running clubs it might add `?is_club_leader=1`
* gym+restaurant with scheduled group eating times
* develop bidding strategies for spectrum auctions by training neural autobidders

