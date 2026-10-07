# Dashboard Metrics Definition

This document outlines the specific metrics that will be surfaced on the landing dashboard of the LogiFlow Platform.

## 1. Real-Time Operational Metrics
| Metric Name | Display Format | Target Threshold | Action Trigger |
| :--- | :--- | :--- | :--- |
| **Pending PO Approvals** | Numeric Badge | 0 | Click to route to PO Approval Screen |
| **Low Stock Alerts** | List / Table | < Reorder Point | Click to generate Draft PR |
| **Shipment Exceptions** | Red Alert Badge | 0 | Click to view delayed/failed shipments |

## 2. Analytical Trends (Trailing 30 Days)
- **Inventory Shrinkage Rate (%):** Line chart comparing system vs physical count variance. (Green = <1%, Yellow = 1-3%, Red = >3%)
- **Average Supplier Rating:** Gauge chart indicating overall vendor health.
- **Fulfillment Cycle Time:** Bar chart showing average hours from Order Receipt to Carrier Dispatch.

## 3. Role-Based Visibility
- **Procurement:** Sees Low Stock, Supplier Ratings, and Pending PRs.
- **Warehouse Manager:** Sees Pending Pick Tasks, Shrinkage, and Dock Capacity.
- **Logistics Director:** Sees total inventory value, global fulfillment times, and overall ROI metrics.
