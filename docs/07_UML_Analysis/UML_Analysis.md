# UML Analysis & System Architecture

This document maps the UML artifacts generated to support the structural and behavioral design of the platform. All diagrams are located in the `/diagrams/` directory.

## 1. Structural Diagrams
- **Domain Model (Class Diagram):** [Domain_Model.puml](../../diagrams/uml_class/Domain_Model.puml)  
  *Defines the core entities (Supplier, PurchaseOrder, InventoryItem) and their relationships.*
- **System Modules (Package Diagram):** [System_Modules.puml](../../diagrams/uml_package/System_Modules.puml)  
  *Illustrates the microservice/module breakdown (Inventory Service, Procurement Service).*

## 2. Behavioral Diagrams
### 2.1 Use Case Diagrams
- **System Use Cases:** [System_Use_Cases.puml](../../diagrams/uml_use_case/System_Use_Cases.puml)
- **Supplier Module:** [Supplier_Module.puml](../../diagrams/uml_use_case/Supplier_Module.puml)
- **Inventory Module:** [Inventory_Module.puml](../../diagrams/uml_use_case/Inventory_Module.puml)

### 2.2 Activity Diagrams
- **Create Purchase Order:** [Create_Purchase_Order.puml](../../diagrams/uml_activity/Create_Purchase_Order.puml)
- **Allocate Inventory:** [Allocate_Inventory.puml](../../diagrams/uml_activity/Allocate_Inventory.puml)
- **Receive Goods:** [Receive_Goods.puml](../../diagrams/uml_activity/Receive_Goods.puml)

### 2.3 Sequence Diagrams
- **Create PO (System Logic):** [Create_Purchase_Order_Sequence.puml](../../diagrams/uml_sequence/Create_Purchase_Order_Sequence.puml)
- **Create Shipment (Carrier API):** [Create_Shipment_Sequence.puml](../../diagrams/uml_sequence/Create_Shipment_Sequence.puml)
- **Stock Reservation (Service Comm):** [Stock_Reservation_Sequence.puml](../../diagrams/uml_sequence/Stock_Reservation_Sequence.puml)

### 2.4 State Machine Diagrams
- **Inventory Item Lifecycle:** [Inventory_Item_State.puml](../../diagrams/uml_state/Inventory_Item_State.puml)
- **PO Lifecycle:** [Purchase_Order_State.puml](../../diagrams/uml_state/Purchase_Order_State.puml)
- **Shipment Lifecycle:** [Shipment_State.puml](../../diagrams/uml_state/Shipment_State.puml)
