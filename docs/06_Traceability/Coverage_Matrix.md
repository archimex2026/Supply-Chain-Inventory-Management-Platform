# Requirements Coverage Matrix

This matrix validates that all functional requirements are covered by both test scenarios (UAT) and system architecture modules.

| Requirement ID | Requirement Description | Sub-System / Module | UML Artifact Reference | UAT Scenario ID | Coverage Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **FR-SM-01** | Supplier creation and management. | Supplier Module | `System_Use_Cases.puml` | UAT-SUP-01 | Covered |
| **FR-SM-02** | Supplier performance score calculation. | Supplier Module | `Data_Flow_View.puml` | UAT-SUP-02 | Covered |
| **FR-PR-01** | Auto-generate PR based on Reorder Point. | Procurement Module | `Create_Purchase_Order.puml`| UAT-PRO-01 | Covered |
| **FR-PR-02** | PO Approval workflow (> $10k). | Procurement Module | `Purchase_Order_State.puml` | UAT-PRO-02 | Covered |
| **FR-IM-01** | Real-time stock update upon Goods Receipt. | Inventory Module | `Receive_Goods.puml` | UAT-INV-01 | Covered |
| **FR-IM-02** | Quarantine functionality. | Inventory Module | `Inventory_Item_State.puml` | UAT-INV-02 | Covered |
| **FR-WH-01** | Logical to physical bin mapping. | Warehouse Module | `Entity_Relationship_Diagram.puml`| UAT-WHS-01 | Covered |
| **FR-SH-01** | Generate unique Tracking ID. | Shipment Module | `Create_Shipment_Sequence.puml` | UAT-SHP-01 | Covered |

*Conclusion:* 100% of defined Functional Requirements are covered by architectural design artifacts.
