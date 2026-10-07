# Naming Conventions

To maintain consistency across the hundreds of artifacts, requirements, and diagrams generated for the **LogiFlow Platform**, all team members must adhere to the following naming conventions.

## 1. File Naming
- **Format:** PascalCase with underscores separating logical components.
- **Markdown Files:** `Descriptive_Name_Of_Document.md` (e.g., `Cost_Benefit_Analysis.md`).
- **Diagrams:** `ProcessName_DiagramType.puml` (e.g., `Create_Purchase_Order_Sequence.puml`).
- **Phase Numbering:** Core phase directories and their primary index documents must be prefixed with the phase number (e.g., `01_Project_Initiation`).

## 2. Requirement ID Numbering
All requirements must be uniquely identifiable for the Requirements Traceability Matrix (RTM).

| Requirement Type | Prefix | Example |
| :--- | :--- | :--- |
| **Business Requirement** | `BR-` | `BR-01`, `BR-02` |
| **Stakeholder Requirement** | `SR-` | `SR-WH-01` (Warehouse) |
| **Functional Requirement** | `FR-[Module]-` | `FR-INV-01` (Inventory) |
| **Non-Functional Requirement**| `NFR-[Type]-` | `NFR-PER-01` (Performance) |

**Module Codes:**
- `SUP`: Supplier Management
- `PRO`: Procurement
- `INV`: Inventory
- `WHS`: Warehouse
- `SHP`: Shipment

## 3. Business Rule ID Numbering
Business rules define the constraints of the system.
- **Format:** `BRul-[Module]-[Number]`
- **Example:** `BRul-PRO-02` (Procurement Rule 2)

## 4. Use Case & User Story Numbering
- **Use Cases:** `UC-[Number]` (e.g., `UC-05: View Inventory`)
- **User Stories:** `US-[Module]-[Number]` (e.g., `US-INV-03`)
- **Acceptance Criteria:** Typically nested under the User Story, but if standalone: `AC-[US-Number]-[Sub-Number]`.

## 5. Test Scenarios (UAT)
- **Format:** `UAT-[Module]-[Number]`
- **Example:** `UAT-SHP-01` (Shipment test scenario)
