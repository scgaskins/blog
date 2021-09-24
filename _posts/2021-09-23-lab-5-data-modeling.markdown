---
layout: post
title:  "Lab 5 Data Modeling"
author: Sammy
---
To convert the different elements of the scenario into entities, I started by looking at every item that acted on another item or was acted upon. For example, items are listed by the owner and purchased by customers, so I made items, customers, and the owner all entities. To refine these entities, I looked at the attributes each entity might have. In doing so, I saw that items in a customer's cart had additional attributes, such as the quantity the customer purchased, that ordinary items didn't have. Because of this, I split cart items and regular items into two separate entities, joined by a relationship. I also noted that the orders themselves have attributes, so I also made them an entity, joined to a customer and cart items. I was then able to produce the following model in Lucid Chart.

![draw-model](/blog/Images/Lab5LucidChartModel.png)

Translating these items to SQL in Vertabelo was fairly straightforward. Each entity on the entity diagram corresponded pretty directly to a table in the SQL file. I did notice that the owner entity wasn't really needed since there is only one owner and the owner has no notable attributes, so I left the owner out of my schema.

![schema](/blog/Images/Lab5VertabeloModel.png)

I think that this data representation captures the necessary elements of the scenario without needless detail.
