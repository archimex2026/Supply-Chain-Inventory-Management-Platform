# KPI Catalog & Definitions

## 1. Procurement KPIs
- **KPI-PRO-01: Purchase Order Cycle Time**
  - *Definition:* Average time from PR creation to PO dispatch.
  - *Target:* < 24 hours
  - *Data Source:* `PurchaseOrder.created_date` vs `PurchaseOrder.dispatch_date`

- **KPI-PRO-02: Supplier On-Time Delivery (OTD)**
  - *Definition:* Percentage of orders delivered on or before the agreed date.
  - *Target:* > 95%
  - *Data Source:* `Shipment.expectedDelivery` vs actual `GoodsReceipt.date`

## 2. Inventory KPIs
- **KPI-INV-01: Inventory Accuracy Rate**
  - *Definition:* Variance between physical counts and system quantities.
  - *Target:* > 99%
  - *Data Source:* Cycle count adjustment logs.

- **KPI-INV-02: Stockout Rate**
  - *Definition:* Percentage of times an item is out of stock when requested.
  - *Target:* < 2%

## 3. Warehouse KPIs
- **KPI-WHS-01: Order Picking Accuracy**
  - *Definition:* Percentage of orders picked without errors.
  - *Target:* 99.5%

## 4. Reporting Requirements
- Daily automated email summary to Logistics Manager.
- Real-time dashboard view for Procurement Officers.
