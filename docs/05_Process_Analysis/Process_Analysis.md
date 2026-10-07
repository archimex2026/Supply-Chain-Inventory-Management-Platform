# Process Analysis (AS-IS & TO-BE)

This document serves as the index and explanatory text for the Business Process Modeling Notation (BPMN) diagrams located in the `/diagrams/bpmn/` directory.

## 1. Procurement Process
- **AS-IS Summary:** Highly manual, email-driven, frequent delays in management approval.
- **TO-BE Diagram:** [Procurement_Process_TO_BE.puml](../../diagrams/bpmn/Procurement_Process_TO_BE.puml)
- **Key Improvements:** Auto-approval thresholds (<$10k), system-generated Draft PRs.

## 2. Order Fulfillment Process
- **AS-IS Summary:** Paper pick lists, visual search for bin locations, manual tracking number entry.
- **TO-BE Diagram:** [Order_Fulfillment_TO_BE.puml](../../diagrams/bpmn/Order_Fulfillment_TO_BE.puml)
- **Key Improvements:** Mobile app for pick tasks, directed put-away/picking via system routing.

## 3. Goods Receiving Process
- **AS-IS Summary:** No system verification of received vs ordered.
- **TO-BE Diagram:** [Goods_Receiving_Process_TO_BE.puml](../../diagrams/bpmn/Goods_Receiving_Process_TO_BE.puml)
- **Key Improvements:** Immediate quarantine tagging for damaged goods, real-time ledger updates.

## 4. Inventory Adjustment Process
- **TO-BE Diagram:** [Inventory_Adjustment_Process_TO_BE.puml](../../diagrams/bpmn/Inventory_Adjustment_Process_TO_BE.puml)
- **Key Improvements:** Automated managerial escalation for adjustments >$500.

## 5. Supplier Evaluation Process
- **TO-BE Diagram:** [Supplier_Evaluation_Process_TO_BE.puml](../../diagrams/bpmn/Supplier_Evaluation_Process_TO_BE.puml)
- **Key Improvements:** 100% automated calculation using On-Time Delivery and Quality Pass metrics.
