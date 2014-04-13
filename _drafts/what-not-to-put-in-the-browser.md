---
layout: post
category : application design
tagline: ""
tags : [application design, single page app]
---
{% include JB/setup %}

Developers will sometimes make what I consider to be a mistake when designing single-page apps, or even just a very javascript-heavy web page.  The mistake they make is that they put the logic for complex domain operations into the browser.  I define "complex" here as involving more than one domain object (actually aggregate root) and/or more than than one operation.  What does this look like?

Let's say we are working on an application that is used to schedule appointments.  So we schedule an appointment, and then if that appointment is successfully scheduled, we

I've seen this a couple of times now, so I thought it would be a good thing to write about.
