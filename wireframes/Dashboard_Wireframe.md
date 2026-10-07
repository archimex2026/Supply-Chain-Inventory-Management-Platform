# Wireframe: Main Dashboard

*This document provides a text-based structural representation (mockup) of the LogiFlow Platform Dashboard.*

---

## 🖥️ Screen Layout: KPI Dashboard

**[Header Navigation]**
`[Logo: LogiFlow]` | `Search...` | `🔔 Notifications (3)` | `👤 User Profile (Admin)`
*Menu:* `Dashboard` | `Suppliers` | `Procurement` | `Inventory` | `Warehouse` | `Shipments`

---

**[Quick Stat Cards (Top Row)]**
- 📦 **Total Inventory Value:** $450,200 (↑ 2% this week)
- 🛒 **Pending PO Approvals:** 5 (Action Required)
- ⚠️ **Low Stock Items:** 12 (Critical)
- 🚚 **Shipments in Transit:** 34

---

**[Main Content Area]**

**Left Column: Inventory Health (Chart Area)**
```text
[ Bar Chart Placeholder ]
X-Axis: Product Categories (Electronics, Perishables, Packaging)
Y-Axis: Quantity on Hand vs Reorder Point
```

**Right Column: Recent Activity Feed**
- 🟢 *10:45 AM* - Goods Receipt processed for PO-99201. (Warehouse A)
- 🔴 *09:30 AM* - Stock for SKU-1002 dropped below ROP. Draft PR generated.
- 🟡 *08:15 AM* - PO-99215 ($12,000) awaits Manager Approval.

---

**[Bottom Row: Data Table - Low Stock Alerts]**
| SKU | Product Name | Qty on Hand | Reorder Point | Action |
| :--- | :--- | :--- | :--- | :--- |
| SKU-1002 | Widget A | 15 | 50 | `[ Create PR ]` |
| SKU-4055 | Packaging Box C | 200 | 500 | `[ Create PR ]` |
| SKU-9932 | Sensor V2 | 0 | 10 | `[ Expedite Order ]`|

---
