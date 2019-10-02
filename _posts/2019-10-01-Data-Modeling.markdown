---
layout: post
author: "Eric Pinter"
title:  "Data Modeling"
date:   2019-10-01 08:00:00 -0500
categories: Databases
---

This was an interesting lab because there was a lot of room for interpretation, which I expect is extremely realistic for database design given a non-specific 'normal person' view of what the database ought to be able to do. I decided to minimize the number of tables and not include unnecessary connections between them. I was also tempted to settle on this because of the fact that anyone who's asking a student in their first semester of studying databases *probably* isn't working with more than a couple thousand transactions a day, and so even very complex queries will never take too long. This all means that there are a couple of things which we might have to calculate at run-time, but it reduces the complexity of the schema significantly. I made a slight exception in marking whether or not a bid was the winning bid. This may, in practical terms, not be necessary, but it provides an easy way to make most queries much easier by juggling that value when a new bid is placed. A real, scalable solution would be to use something like a view, especially if our data needs were to do more than just determine the winning bid and operate on its cash amount.
![A simple relational layout]({{site.baseurl}}/assets/img/Lab5draw.png)
I'm not quite sure how much separating the ER diagram and database schema is helpful, though I can see that more interesting differences would appear for larger and more complex layouts than mine. It may also just be that databases are in my blood, but it seems to me that reading the data-flows from a schema and creating a schema from scratch are roughly as hard as doing the same for an ER diagram. Also, I'm decently confident that the data-flow connections are of the correct cardinality and direction, mostly because Vertabelo only displays the correct fields when you have the connections in the right direction.
![A full schema]({{site.baseurl}}/assets/img/Lab5vertabelo.png)
