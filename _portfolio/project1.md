---
title: Universal Search
subtitle: Increasing the discoverability of SwimTrek's trips, blog posts and other content.
video_name: universal_search
poster: assets/video/universal_search.png

caption:
  title: Universal Search
  subtitle: Increasing Discoverability
  thumbnail: assets/video/universal_search.png
---

**As the number of products you offer grows so too does the challenge of helping
customers discover them. In this project we developed a site-wide search system
enabling SwimTrek's customers to quickly find their ideal trip and any other
content relevant to their interests.**

Since we built SwimTrek's site, in 2015, they have significantly increased the
number of package holidays they offer, as well as adding hundreds of blog posts
and other staff-generated pages as part of their content marketing strategy. By
2020 it was becoming increasingly clear that the site's existing browsing tools
were insufficient to navigate this large body of content. To address this we
reviewed various search interfaces with SwimTrek and arrived at a design that
incorporated the following features:

- **a site-wide, keyword search-box**
  - similar to that on popular e-commerce sites, with...
  - clickable search suggestions updated as the user types
  - clickable result previews enabling the full search interface to be skipped 
- **a Google-inspired search results interface**
  - with multiple "verticals": _All_, _Trips_, _Dates_, _Blog_ and _Other_
  - thus allowing the user to quickly view keyword matches for records of a
    particular type
- **an AirBnb-inspired filter interface**
  - filter buttons that both launch the filter's menu and display a summary of
    its current setting 
  - result count previews indicating how many results will be shown with the
    current settings
  - interactive histograms for range-based filters like price and trip duration

To power the search interface we evaluated several technologies before settling
on **Algolia**, a hosted search-as-a-service provider with the indexing and
querying features we needed at a reasonable monthly price. The search interface
is implemented as a **Vue.js** Single Page Application (SPA) that is loaded as
part of the site's standard JavaScript bundle, so that it can take over control
of the page instantly when search is invoked. When combined with the speed of
Algolia's API this makes the search interface incredibly snappy, providing an
excellent user experience.

Since its introduction, the Universal Search interface has proved to be very
popular with the site's visitors, who now routinely use it as their main
site-navigation tool. The breadth of content viewed by a typical visitor has
increased significantly, demonstrating that the project has been successful in
increasing discoverability. Furthermore, search analytics have provided
SwimTrek's marketing and product teams with valuable insights into how customers
choose their ideal holiday, highlighting an additional benefit of a
fully-featured search interface.

---

{:.list-inline}
- **Date**: August 2020
- **Client**: SwimTrek
