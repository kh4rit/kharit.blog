---
layout: post
title: What is EDM? (for enterprise architecture)
author: Vasiliy
categories: architecture
tags: [enterprise-architecture, architecture]
---

EDM or Enterprise Data Model allows applications within an Enterprise to speak
to each other in the same language.

From my perspective EDM is the next step after MDG (Master Data Governance)
where MDG aligns between different systems masterdata (like business partners
and materials) and EDM makes a step further to align transactional data (like
sales orders and deliveries).

EDM is becoming a popular topic as enterprises do not want to lock themselves
to a single vendor, but still want applications from different vendors to speak
with each other.

---

Is it some product or category of products? There can be some supportive
products for data translation (like SAP One Domain Model) and modelling, but
this is more an abstract or logic construct. Real world implementation could
look like a documentation discribing which documents you have within your
organization and which rules should be followed to change them or add new ones.

Does it mean we can't use vendor-provided data model? Not really. The concept
of EDM usuall comes with translation of vendor-specific data to EDM.

---

With EDM even if you have a multiple warehouse management systems from
different vendors, upon uploading the data to BW system you can translate it to
a single EDM. Thus, ensuring BW reports will work independently of which system
is the source of data, which will unlock business to use global data for
decision-making.
