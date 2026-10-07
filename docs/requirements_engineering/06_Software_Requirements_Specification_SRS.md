# Software Requirements Specification (SRS)

## 1. Introduction
### 1.1 Purpose
The purpose of this document is to define the software requirements for the Supply Chain & Inventory Management Platform. This document outlines the functional and non-functional requirements to guide the development and QA teams.

### 1.2 Scope
This system covers Procurement, Inventory Control, Warehouse Operations, and Shipment Management.

## 2. Functional Requirements
### 2.1 Supplier Management
- **FR-SM-01:** The system shall allow authorized users to create, read, update, and deactivate supplier profiles.
- **FR-SM-02:** The system shall calculate a supplier performance score based on on-time delivery rates and defect rates.

### 2.2 Procurement
- **FR-PR-01:** The system shall auto-generate a Purchase Request (PR) when an inventory item falls below its defined Reorder Point.
- **FR-PR-02:** The system shall enforce a two-step approval workflow for Purchase Orders (POs) exceeding $10,000.

### 2.3 Inventory Management
- **FR-IM-01:** The system shall update the "Quantity On Hand" in real-time when Goods Receipts (GR) are processed.
- **FR-IM-02:** The system shall allow users to quarantine inventory items (status='Quarantined'), preventing their allocation to outbound shipments.

### 2.4 Warehouse & Shipment
- **FR-WH-01:** The system shall map physical warehouse locations (Aisle, Rack, Bin) to logical system locations.
- **FR-SH-01:** The system shall generate a unique Tracking ID for each confirmed shipment.

## 3. Non-Functional Requirements
- **NFR-PER-01 (Performance):** The system shall load the main inventory dashboard within 2 seconds for up to 10,000 concurrent items.
- **NFR-SEC-01 (Security):** All user passwords shall be hashed using bcrypt or a similar industry-standard algorithm.
- **NFR-AVA-01 (Availability):** The system shall guarantee 99.9% uptime during standard business hours (08:00 - 20:00).
- **NFR-AUD-01 (Auditability):** The system shall maintain an immutable audit log of all inventory quantity adjustments.
