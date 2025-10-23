# Adventure Works - Analytics Dashboard
## Overview
This project uses the "Adventure Works" public dataset to build a comprehensive, multi-page analytical dashboard

The goal is to move beyond simple reporting and practice advanced analytical techniques, to uncover deeper business insights. The project also focuses on creating a custom, application like UI/UX

## Dataset
Represents a multinational company, "Adventure Works," that sells bicycles and accessories

The dataset includes information on products, customers, sales territories, and order details across multiple years

[Adventure Works](https://www.kaggle.com/datasets/ukveteran/adventure-works)

## Built with
- Power BI Desktop
- Power Query
- DAX

## Key Features vs Basic Dashboard
RFM analysis: customer segmentation based on Recency, Frequency, and Monetary

Basket Analysis: tool to discover which products are frequently purchased together, using the "Disconnected Slicer" pattern

Navigation: left-side navigation panel using icons and Bookmarks to move between pages

Custom Tooltips: tooltips provide extra context on hover

Azure Map: using a GeoJSON reference layer to visualize sales by country

RLS: roles are configured to restrict data access (by sales territory)

## Files
- [adv.pbix](adv.pbix) — Power BI project file
- [adv.pdf](adv.pdf) — PDF-version
- [/data](/data) — Folder containing all Datasets

## Note
This Power BI file is configured to load data directly from this GitHub repository via the web

As long as you have an active internet connection, the data will refresh successfully. There is no need to edit local paths or parameters

## Key Insights
- Shorts are a consistent return problem. Over the last three years, "Shorts" are the #1 most returned product overall in both North America and Europe. Even though they only spiked as a yearly leader once (Europe 2017), this finding shows they are being consistently returned across both regions, which eats into profits.

- When a customer buys a specific "Tire", they also buy the matching "Tire Tube" in the same order (around 60-80% of the time). The company should create "Tire + Tube" bundles to make buying easier and potentially increase sales.

- The business model is not about "Champions". The RFM analysis shows that this business does not rely on "Classic Champions". Revenue is driven by other groups. The company's strategy should be to:

  - Re-engage the large "Hibernating" segment before they become "Lost."

  - Retain the "Big Spenders."

  - Improve the retention of "New Customers" to get them to make a second purchase.
