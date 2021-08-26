---
title: Trip Timetable
subtitle: Simplifying operations with a custom graphical interface.
video_name: trip_timetable
poster: assets/video/trip_timetable.png

caption:
  title: Trip Timetable
  subtitle: Simplifying Operations
  thumbnail: assets/video/trip_timetable.png
---

**In this project we built a custom, horizontal calendar interface tailored to
the needs of SwimTrek's operations team.**

SwimTrek's operations team take care of trip logistics, ensuring that personnel
and equipment are in the right place at the right time, for hundreds of
departures all around the globe. To provide an at-a-glance overview of the
year's trips, they had developed a colour-coded, shared spreadsheet that
displayed salient information about each trip in a horizontal timeline.

While very useful, this spreadsheet approach had some significant shortcomings.
Chief among these was the fact that the information in the spreadsheet was not
linked to that in the website's database, meaning lots of manual copying back
and forth, with the potential for costly human error posing a significant
business risk. Consequently, SwimTrek asked us to build a similar interface into
the admin area of their site, with the following features:

- **intuitive UI**
  - the same layout and colour coding as the spreadsheet staff were familiar with
  - drag-and-drop adjustment of trip start and end dates
  - the ability to filter by multiple trip properties
  - a fly-out form allowing the most important information to be set
- **issue management**
  - automatic detection of resourcing issues, e.g., guides being double-booked
    or working too many consecutive days
  - the ability to add manual issues
  - the ability to dismiss/restore issues of either type
- **data management**
  - the website's database as the "single source of truth", with all data
    fetched and saved to it
  - collaborative editing, with indicators to show which users are working on
    the same year, and with their edits being instantly visible without page
    reloads

We built the interface as a **Vue.js** Single Page Application (SPA) backed by a
private API we built on top of the site's departure management system. We used
the **FullCalendar** library to power the timeline UI, and **Pusher** to power
the collaborative editing, with messages being pushed to all connected clients
whenever edits are made to the year they are working on.

The new interface has been a big hit with the operations team who now use it as
their main tool for day-to-day activities. They report that it saves them a lot
of time over the old spreadsheet approach, and has made the work less stressful
thanks to the automatic issue detection. The interface has also proved to be a
useful planning tool for the product team, who use it to explore scenarios for
future trips.

---

{:.list-inline}
- **Date**: April 2019
- **Client**: SwimTrek

