---
description: Adobe provides various calculated metrics that you can use. This page lists those metrics and their intended uses.
title: Reference  basic functions
feature: Calculated Metrics
exl-id: 1a49435c-96d1-4617-bd1a-a5d3b74e3ebd
---
# Default Calculated Metrics

Adobe Analytics provides various Calculated Metrics to cover the most common use-cases. These Calculated Metrics are available by default in Analysis Workspace.

Following is a list of each Calculated Metric that is provided by Adobe, with its intended function and the underlying formula used to calculate it:

>[!NOTE]
>
>In addition to the default Caluclated Metrics described on this page, you can also add additional Calculated Metrics to a Report Suite.  
>
>You can:
> * Add default Calculated Metrics for Streaming Media, as described in [Calculated metrics](/https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/calculated-metrics.html) 
> * Create custom Calculated Metrics from existing Metrics, as described in [Calculated and Advanced Calculated (Derived) Metrics](/help/components/c-calcmetrics/cm-overview.md).


|Calculated Metric Name | Function | Formula |
|---------|----------|---------|
| Bounce Rate | The ratio of visits that contained exactly one hit compared to the number of visits on that page. This can help you understand which dimension items have the highest bounce rate, or to see an aggregated total bounce rate of your site over time. | Bounce Rate |
| Revenue / Visitor | The average amount of revenue generated by each individual visitor to the site. | <p>Revenue</p><p>/</p><p>Unique Visitors</p> |
| Orders / Visitor | The average number of orders or transactions generated by each individual visitor to the site | <p>Default Orders</p><p>/</p><p>Visitor</p> |
| Revenue / Visits | The average amount of revenue generated by a single visit to the site. | <p>Revenue</p><p>/</p><p>Unique Visits</p> |
| Revenue / Order | The average amount of revenue generated by each completed transaction or order on the site. | <p>Revenue</p><p>/</p><p>Order</p> |
| Orders / Visits | The percentage of visits to the site that result in a completed transaction. | <p>Order</p><p>/</p><p>Visits</p> |
| Page Views / Visits  | The average number of pages a user views during a single visit to the site. | <p>Page Views</p><p>/</p><p>Visits</p> |
| Visits / Visitor | The average number of visits a unique visitor makes to the site.  | <p>Visits</p><p>/</p><p>Unique Visitors</p> |
| Reloads / Pageviews | The percentage of page views that resulted in a reload or refresh of the page. | <p>Reloads</p><p>/</p><p>Page Views</p> |
| Weighted Bounce Rate | Function | if(visits>percentile(visits),bouncerate,0) |
| Order Assists | The number of times a channel or source contributed to a customer's journey towards making a purchase, but did not result in the final purchase. | <p>Orders (Participation\|Visit)</p><p>-</p><p>Orders</p> |
| Exit Rate | The percentage of visitors who leave the site after viewing a particular page. | <p>Exits</p><p>/</p><p>Visits</p> |
| Entry Rate | The percentage of visitors who entered the site on a given page, compared to the total number of sessions on the site. | <p>Entries</p><p>/</p><p>Visits</p> |
| Average Time on Site | The average amount of time a visitor spends on the site before leaving or navigating away. | Average Time Spent on Site (Seconds) |
| Time Spent/User (State) | The length of time that the average visitor spends in a particular State while on the site | Time Spent per Visitor (Seconds) metric + Mobile App segment |
| Users (Mobile) | The total number of users of a mobile app | Unique Visitors metric + Mobile App Users segment |
| App Users | The total number of users of a mobile app | Unique Visitors metric + Mobile App segment |
| State Views | The number of views to the different states or screens of the app | Page Views metric + Mobile App segment |
| Actions | The total number of actions taken in the app | Custom Link Instances metric + Has an Action segment |
| Acquisition Link Clicks | The number of times people click a link that is designed to drive traffic to the site. | Campaign Click-throughs metric |
| Page Velocity | The number of additional page views that a piece of content generates. This can help you determine which content drives additional engagement. | <p>Page Views</p><p>/</p><p>Visits</p> |
| Conversion Rate | The percentage of visitors who took a desired action, such as made a purchase. | <p>Orders</p><p>/</p><p>Visits</p> |
| Average Session Length (Mobile) | The average amount of time visitors spend on the site during a single session. | Blank |
| Experience Cloud ID coverage | The percentage of visitors who have an Experience Cloud ID. | <p>Visitors with Experience Cloud ID</p><p>/</p><p>Unique Visitors</p> |
| Content Velocity | The speed at which new content is created and published on the site and how quickly it generates user engagement. | <p>Page Views</p><p>/</p><p>Visits</p> |
| ITP 2.1 Unique Visitors / Unique Visitors | The percentage of unique visitors using a browser affected by ITP 2.1 cookie limitations. In other words, customers not using a CNAME implementation. (This applies to customers setting cookies via client-side JavaScript.) | <p>Unique Visitors metric + ITP Visitors segment</p><p>/</p><p>Unique Visitors</p> |
| Unique Visitors / Unique Visitors returning after 7 days  | The percentage of unique visitors who are returning after a period of 7 or more days. | <p>Unique Visitors metric + Users returning after 7 days segment</p><p>/</p><p>Unique Visitors</p> |
| Page Views / Unique Visitor | The average number of pages viewed for each unique visitor to the site. | <p>Page Views</p><p>/</p><p>Unique Visitors</p> |
| Visits / Visitors | The average number of visits a unique visitor makes to the site . | <p>Visits</p><p>/</p><p>Unique Visitors</p> |
| Estimated Unique Visitors (ITP 2.1) | <p>For ITP visitors (users on Safari browsers) divide Unique Visitors by 2 or less.</p><p>This assumes you are setting cookies using client-side JavaScript (not using a CNAME implementation). Implementations that set cookies using client-side JavaScript were impacted starting with ITP 2.1. See: [https://webkit.org/blog/8613/intelligent-tracking-prevention-2-1/](https://webkit.org/blog/8613/intelligent-tracking-prevention-2-1/)</p> | <p>Unique Visitors metric + ITP Visitors (ITP 2.1, Non-CNAME implementations) segment</p><p>/</p><p>Unique Visitors metric + Non-ITP Visitors (ITP 2.1, Non-CNAME implementations) segment</p> |
| Page Views / Estimated Unique Visitors (ITP 2.1) | The average number of pages viewed for Estimated Unique Visitors (ITP 2.1). | <p>Unique Visitors metric + ITP Visitors (ITP 2.1, Non-CNAME implementations) segment</p><p>/</p><p>Unique Visitors metric + Non-ITP Visitors (ITP 2.1, Non-CNAME implementations) segment</p> |

{style="table-layout:auto"}