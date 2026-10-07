# Wireframe: Purchase Order (PO) Details

*This screen displays the detailed view of a specific Purchase Order for approval or tracking.*

---
**[Header Navigation]**
`[Logo: LogiFlow]` | `Search PO...` | `👤 (Manager)`
`← Back to PO List`

---
**[Top Section: PO Summary Card]**
## PO-99215 
**Status:** 🟡 `Pending Approval`
**Supplier:** TechCorp Components Inc. (Rating: ⭐ 4.5/5)
**Created By:** Jane Doe (Procurement) | **Date:** 2026-10-07
**Expected Delivery:** 2026-10-14

---
**[Middle Section: Line Items]**

| Item # | SKU | Description | Qty | Unit Price | Total Price |
|---|---|---|---|---|---|
| 1 | SKU-1002 | Widget A | 1,000 | $10.00 | $10,000.00 |
| 2 | SKU-9932 | Sensor V2 | 500 | $5.00 | $2,500.00 |
| | | | | **Subtotal:** | $12,500.00 |
| | | | | **Tax (19%):**| $2,375.00 |
| | | | | **Total:** | **$14,875.00** |

---
**[Approval Workflow Panel - Right Sidebar]**
**Rule Triggered:** Total > $10,000 requires Manager Approval.

`[ ✔️ APPROVE PO ]`   `[ ❌ REJECT PO ]`

*Add Comment:*
`[ Textbox: Type reason for rejection or approval note here... ]`

---
**[Activity Log]**
- *2026-10-07 09:30* - PO Created by Jane Doe.
- *2026-10-07 09:30* - Routed for Manager Approval (Total > 10k).
