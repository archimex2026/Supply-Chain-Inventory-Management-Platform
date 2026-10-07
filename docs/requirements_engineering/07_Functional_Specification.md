# Functional Specification Document (FSD)

## 1. Introduction
This FSD translates the Software Requirements Specification (SRS) into specific functional behavior, detailing how the system will operate from a user's perspective.

## 2. Module: Inventory Management
### 2.1 Function: Stock Allocation
**Trigger:** An outbound shipment is created.
**System Behavior:**
1. System queries `QuantityOnHand` for requested SKU.
2. If `QuantityOnHand` >= `RequestedQty`, system subtracts `RequestedQty` from `AvailableQty` and adds it to `AllocatedQty`.
3. System logs transaction in `InventoryLedger`.
**Exception:** If `QuantityOnHand` < `RequestedQty`, system displays error: *"Insufficient stock for allocation"* and prompts for backorder creation.

### 2.2 Function: Cycle Counting
**Trigger:** User initiates cycle count for Aisle B.
**System Behavior:**
1. System locks inventory movements for Aisle B (Status = `Count_In_Progress`).
2. System generates a blind count sheet (SKUs listed, but expected quantities hidden).
3. User inputs physical counts.
4. System calculates variance. If variance > 5%, Manager Approval workflow is triggered.
5. Upon approval, system updates `QuantityOnHand` and unlocks Aisle B.

## 3. Module: Supplier Management
### 3.1 Function: Auto-Rating Calculation
**Trigger:** End of month batch job.
**System Behavior:**
1. System retrieves all closed POs for Supplier X in the last 30 days.
2. Calculates % of POs delivered on time (Weight: 60%).
3. Calculates % of items passing quality check (Weight: 40%).
4. Updates `Supplier.performanceRating`.
