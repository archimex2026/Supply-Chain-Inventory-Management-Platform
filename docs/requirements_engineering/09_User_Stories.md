# User Stories

## Epic 1: Automated Procurement
**US-PR-01: Auto-generate Purchase Requests**
As a Procurement Officer,
I want the system to automatically generate a Purchase Request when an item's stock falls below the reorder point,
So that I can quickly review and order stock without manually checking inventory levels daily.

*Acceptance Criteria:*
- System monitors `quantityOnHand` against `reorderPoint`.
- When `quantityOnHand` <= `reorderPoint`, a Draft PR is created.
- The Procurement Officer receives a system notification.

**US-PR-02: PO Approval Workflow**
As a Department Manager,
I want to be notified of Purchase Orders exceeding $10,000,
So that I can review and approve them before they are sent to the supplier.

*Acceptance Criteria:*
- Any PO with `totalAmount` > $10,000 requires explicit approval.
- The PO status remains `Pending Approval` until actioned.
- The PO cannot be exported or emailed to the supplier until the status is `Approved`.

## Epic 2: Inventory Tracking
**US-IM-01: Quarantine Defective Stock**
As a Warehouse Operator,
I want to be able to mark specific inventory items as "Quarantined",
So that they are not accidentally picked and shipped to customers.

*Acceptance Criteria:*
- User can select an inventory item and change its status to `Quarantined`.
- The system prevents allocation of `Quarantined` items to any outbound shipment.
- The item remains in the physical bin but is logically separated in the system.
