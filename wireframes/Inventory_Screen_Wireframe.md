# Wireframe: Inventory Screen

*This screen allows warehouse staff and inventory analysts to view, filter, and adjust stock levels.*

---
**[Header Navigation]**
`[Logo: LogiFlow]` | `Search SKU...` | `🔔 (1)` | `👤 (Analyst)`

---
**[Action Bar]**
`[ + New Adjustment ]`  `[ 🔄 Trigger Cycle Count ]`  `[ 📥 Export CSV ]`

**Filters:** 
`Category: [All ▾]`  `Warehouse: [WH-North ▾]` `Status: [Available ▾]`

---
**[Data Table: Master Inventory List]**

| ⬜ | SKU | Product Name | Category | WH Loc | Qty On Hand | Allocated | Available | Status | Actions |
|---|---|---|---|---|---|---|---|---|---|
| ⬜ | SKU-1002 | Widget A | Elec | A1-B2 | 150 | 50 | 100 | 🟢 Active | `[⋮]` |
| ⬜ | SKU-1003 | Widget Pro | Elec | A1-B3 | 0 | 0 | 0 | 🔴 Out | `[⋮]` |
| ⬜ | SKU-4055 | Box C | Pkg | C4-D1 | 200 | 0 | 200 | 🟡 Quarnt | `[⋮]` |
| ⬜ | SKU-9932 | Sensor V2 | Parts | B2-A1 | 45 | 40 | 5 | 🟢 Active | `[⋮]` |

---
**[Pagination]**
`[◄ Prev]` `Page 1 of 12` `[Next ►]`
