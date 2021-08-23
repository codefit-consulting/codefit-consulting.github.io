---
title: Streamlined Checkout
subtitle: Boosting conversions by keeping things simple.
video_name: streamlined_checkout
poster: assets/video/streamlined_checkout.png

caption:
  title: Streamlined Checkout
  subtitle: Boosting Conversions
  thumbnail: assets/video/streamlined_checkout.png
---

**Once a customer has indicated that they wish to make a purchase, it's
generally a good idea to get out of their way and get them to the "PAY NOW"
button ASAP. In this project we redesigned the SwimTrek checkout experience to
make it as frictionless as possible, especially for returning customers.**

As a result of new EU regulations, SwimTrek needed to add **3D Secure** support
to their card payments which, in turn, necessitated a change of payment
processor. After reviewing options with SwimTrek we agreed to go with
**Stripe**. Given that the move to Stripe required significant rework to the
checkout interface anyway, SwimTrek opted to go with a full redesign, with the
goal of making the time between clicking "BOOK NOW" and "PAY NOW" as short and
pain-free as possible.

We reviewed the informational requirements of the booking process, identifying
any information that could be gathered _after_ the booking was placed, and thus
removed from the checkout. For the remaining information we explored
opportunities to pre-fill the checkout form based on:

- availability search settings prior to pressing "BOOK NOW"
- profile information held on record for the logged in user (if returning)
- available options, e.g., pre-selecting room type if there is only one choice remaining

The resultant design was implemented as a **Vue.js** Single Page Application
(SPA) that interacts with a new private API we built on top of the site's
exiting booking system. The checkout is presented as a simple three-step process
(Log In → Details → Payment), but is flexible enough to deal with multiple
edge cases:

- trips with multiple hotel stays or none at all
- trips with paid or free optional extras to choose from
- customers booking on behalf of others but not attending personally
- customers with account credit to contribute towards the cost of their trip
 
The same interface doubles up as a self-serve edit interface that customers can
use to update their trip _after_ booking (e.g., adding a guest or changing a
room) and is also used by staff to create/update bookings on behalf of telephone
customers, presenting them with additional staff-only options that customers
don't see.

Since launching the new interface, the average time to complete the checkout
process has reduced from three minutes to just one, the number of abandoned
bookings has halved and the proportion of bookings completed by customers
themselves has increased significantly, reducing pressure on sales staff,
especially during busy periods.

---

{:.list-inline}
- **Date**: August 2018
- **Client**: SwimTrek

