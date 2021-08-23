---
title: Availability Search
subtitle: Reducing frustration by allowing customers to summarise their requirements before starting a booking.
video_name: availability_search
poster: assets/video/availability_search.png

caption:
  title: Availability Search
  subtitle: Reducing Frustration
  thumbnail: assets/video/availability_search.png
---

**In this project we designed an intuitive interface that allows customers to
refine the list of trip dates that can meet their requirements, helping them to
avoid the frustration of starting a booking only to discover that their chosen
date is unsuitable.**

SwimTrek give their customers a lot of flexibility in rooming arrangements:
single-supplement, roommate matching, additional non-swimming guests, etc.
However, because trips have a fixed inventory of reserved rooms, the options
that can be offered to a customer must be limited as a trip fills up, in order
to ensure that there are sufficient rooms left to accommodate the target number
of swimmers, and to satisfy additional business constraints.

Automating this process was a key challenge when we originally built SwimTrek's
site. We developed a custom **Room Allocation Engine** that quickly determines
what rooming arrangements can be offered to a customer given their needs and the
current state of the trip. In the original build, the engine was only called
during the checkout process, updating the available room offers after each room
selection. In this project we exposed the Room Allocation Engine via a private
API consumed by our in-page widget and added support for efficient bulk
processing of multiple departures.

The in-page widget was developed using **Vue.js**, and provides a familiar table
interface, but with rows that can be expanded to reveal additional details for a
given trip date. The call-to-action directs the customer to a form that collects
summary-level information about their guests and desired rooming arrangements,
whereupon the system issues an API request, and updates the call-to-action
buttons with messages indicating the suitability of each departure date.

By allowing customers to better explore availability, this enhancement reduced
the number of telephone, chat and email enquiries related to trip capacity,
reducing the burden on office staff and improving customer satisfaction.

---

{:.list-inline}
- **Date**: July 2018
- **Client**: SwimTrek

