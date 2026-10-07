# Business Rules Catalog

This catalog outlines the explicit business rules governing the logic within the Supply Chain & Inventory Management Platform.

## 1. Supplier Rules
- **BRul-SUP-01:** A supplier must provide a valid Tax ID and Banking Information to be set to an `Active` state.
- **BRul-SUP-02:** Suppliers with an average performance rating below 60% over a rolling 90-day period are automatically flagged for `Review`.

## 2. Procurement Rules
- **BRul-PRO-01:** Any Purchase Order (PO) with a total value <= $10,000 is auto-approved if generated from an automated Purchase Request (PR).
- **BRul-PRO-02:** Any PO with a total value > $10,000 requires explicit approval from the Logistics Manager.
- **BRul-PRO-03:** A PO cannot be sent to a supplier whose status is `Inactive` or `Under Review`.

## 3. Inventory Rules
- **BRul-INV-01:** When the `Quantity On Hand` of an active SKU falls below its `Reorder Point`, the system must generate a Draft Purchase Request.
- **BRul-INV-02:** Inventory marked with the status `Quarantined` cannot be allocated to a customer shipment.
- **BRul-INV-03:** Inventory adjustments (increases or decreases) exceeding 10% of the total SKU quantity require an explanatory reason code and Manager approval.

## 4. Warehouse & Shipment Rules
- **BRul-WHS-01:** Goods placed in a storage bin must not exceed the `MaxWeight` limit defined for that specific bin.
- **BRul-SHP-01:** A shipment cannot transition to the `Dispatched` state unless all allocated items are confirmed as picked and packed.
