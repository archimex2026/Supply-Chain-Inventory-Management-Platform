# Data Dictionary

This document defines the properties of the core data entities stored in the database.

## 1. Entity: `InventoryItem`
| Field Name | Data Type | PK/FK | Nullable | Description |
| :--- | :--- | :--- | :--- | :--- |
| `item_id` | INT | PK | No | Unique system identifier for the item. |
| `sku` | VARCHAR(50) | - | No | Stock Keeping Unit, human-readable barcode value. |
| `name` | VARCHAR(100) | - | No | Descriptive name of the product. |
| `qty_on_hand` | INT | - | No | Physical quantity currently sitting in the warehouse. |
| `allocated_qty` | INT | - | No | Quantity reserved for pending outbound shipments. |
| `reorder_point` | INT | - | No | Threshold that triggers a draft Purchase Request. |
| `status` | VARCHAR(20) | - | No | Enum: 'Active', 'Quarantined', 'Discontinued'. |

## 2. Entity: `PurchaseOrder`
| Field Name | Data Type | PK/FK | Nullable | Description |
| :--- | :--- | :--- | :--- | :--- |
| `po_id` | INT | PK | No | Unique PO number. |
| `supplier_id`| INT | FK | No | Reference to `Supplier` table. |
| `created_date`| DATETIME | - | No | Timestamp of creation. |
| `total_amount`| DECIMAL(10,2)| - | No | Total financial value of the PO. |
| `status` | VARCHAR(20) | - | No | Enum: 'Draft', 'Pending_Approval', 'Approved', 'Dispatched', 'Fulfilled'. |

## 3. Entity: `WarehouseBin`
| Field Name | Data Type | PK/FK | Nullable | Description |
| :--- | :--- | :--- | :--- | :--- |
| `bin_id` | INT | PK | No | Unique Bin ID. |
| `aisle` | VARCHAR(10) | - | No | Aisle identifier (e.g., A1, B4). |
| `max_weight` | DECIMAL(8,2) | - | No | Maximum weight capacity in kg. |
