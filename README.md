# Amazon Sales Dashboard (Power BI)

An interactive Power BI dashboard for analyzing Amazon order and sales data, with dedicated views for **Overview**, **Products**, and **Product View**.

## Dashboard Preview

![Amazon Sales Dashboard Overview](./screenshots/dashboard-overview.png)

## Features

- **KPIs**
  - All Sale: 120K
  - Filter_Sale: 89M
  - Toggle between **Sales** and **Units**
- **Status Filter (Slicer)**
  - Cancelled, Pending, Pending – Waiting for Pick Up, Shipped, Shipped – Damaged, Shipped – Delivered to Buyer, Shipped – Lost in Transit, Shipped – Out for Delivery, Shipped – Picked Up, Shipped – Rejected by Buyer, Shipped – Returned to Seller
- **Sales by City** — horizontal bar chart (Bengaluru, Hyderabad, Mumbai, New Delhi, Chennai, Pune, Kolkata, Gurugram)
- **Sales by State** — horizontal bar chart (Maharashtra, Karnataka, Tamil Nadu, Telangana, Uttar Pradesh, Delhi, Kerala, West Bengal)
- **Total Sale Trend** — area/line chart tracking sales over time (Apr 2022 – Jun 2022)
- **Product Catalog Panel** — product thumbnails with category names (Baby Carriers, Bag Organizers, Boys Belts, Boys Boxer Shorts, Boys Clothing Sets, Boys Dhotis, Boys Dungarees, Boys Ethnic Wear, etc.)

## Tech Stack

- **Power BI Desktop**
- **DAX** measures (Sales Amount, Units, filtered aggregations)
- Data model with **Orders**, **Products**, and **Location** tables

## Data Fields (Assumed Schema)

| Field | Description |
|---|---|
| Order ID | Unique identifier for each order |
| Order Date | Date of transaction |
| Status | Order fulfillment status |
| City / State | Customer location |
| Category | Product category |
| Sales Amount | Revenue per order |
| Units | Quantity sold |
| Product Image / SKU | Product reference |

## Purpose

Track e-commerce sales performance across Indian cities and states, monitor order fulfillment/return status, and identify top-performing product categories over time.

## How to Use

1. Open the `.pbix` file in Power BI Desktop.
2. Use the **Status** slicer to filter by order fulfillment stage.
3. Toggle between **Sales** and **Units** to change KPI/chart context.
4. Switch tabs (**Overview / Products / Product View**) for deeper drill-downs.

## Folder Structure

```
project/
├── README.md
└── screenshots/
    └── dashboard-overview.png
```
