# Production-Commercial-Dashboard

A web-based dashboard for monitoring inventory, production, and shipment activity across the mill. Built to give operations and commercial teams a shared, real-time view of how inventory is flowing from production through to customer shipment.

## Purpose

This dashboard consolidates data that currently lives in separate systems so the team can answer key operational questions at a glance:

- Where is our inventory sitting right now?
- How long has it been sitting there?
- Who are our active customers based on recent shipments?
- How are current production runs aligning with inventory levels and demand?

## Features

### Inventory by Bay
Real-time view of on-hand inventory broken out by storage bay. Supports drill-down by product, grade, size, and heat number. Designed to help yard and shipping teams locate material quickly and identify capacity issues before they become bottlenecks.

### Aging Inventory
Tracks how long material has been in inventory, with configurable aging buckets (e.g., 0–30, 31–60, 61–90, 90+ days). Highlights slow-moving stock so commercial and production teams can take action before material becomes a write-down risk.

### Customer Shipment Insights
Surfaces top customers, shipment volume, and shipment frequency from historical shipment data. Helps commercial understand where material is going and supports forecasting and account management.

### Production Run Tracking
Visibility into active and recent production runs, tied back to resulting inventory. Lets the team see how production decisions translate into on-hand stock and shipped tons, and whether we're building the right mix.

### Inventory Management Performance
Roll-up metrics that tie the above together — turns ratio, days-on-hand, build-to-ship cadence, and aging trend over time — so leadership can see whether our inventory strategy is actually working.

## Architecture

_To be defined. Target stack:_

- **Frontend:** TBD (React + Iron UI components likely)
- **Backend / Data:** Nucor Data Hub (NDH) via Databricks
- **Authentication:** Entra ID
- **Hosting:** TBD (Azure)
- **AI/LLM features (if applicable):** Azure AI Foundry endpoints with managed identity

## Status

🚧 Early development — repository scaffolding in progress.

## Roadmap

- [ ] Define data sources and access patterns (NDH tables, MIPS, shipment systems)
- [ ] Wireframe primary views (Inventory by Bay, Aging, Customers, Production)
- [ ] Stand up authentication via Entra ID
- [ ] Build out first view: Inventory by Bay
- [ ] Layer in aging analytics
- [ ] Add shipment/customer view
- [ ] Add production run view
- [ ] Combined performance dashboard

## Contact

**Owner:** Jordan Hamblin
**Team:** _TBD_
