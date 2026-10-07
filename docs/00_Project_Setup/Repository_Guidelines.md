# Repository Guidelines

## 1. Purpose
This document establishes the rules and best practices for contributing to the **Supply Chain & Inventory Management Platform** documentation repository. Maintaining a clean and structured repository ensures that Business Analysts, System Analysts, and Developers can easily navigate the project artifacts.

## 2. Directory Structure Governance
The repository strictly follows the 12-Phase Project Lifecycle model. All new documents MUST be placed in their corresponding phase folder under `/docs/`:
- **Phase 00 - Phase 11:** Documentation and analysis markdown files.
- **/diagrams:** All PlantUML (`.puml`) source files, categorized by diagram type (BPMN, UML_Class, UML_Sequence, etc.).
- **/wireframes:** Text-based or image-based UI mockups.
- **/templates:** Reusable markdown templates (e.g., BRD, Use Cases).

*Rule:* Do not create root-level folders without approval from the Lead Business Analyst.

## 3. Contribution Workflow
1. **Branching:** Create a new branch for any significant addition. 
   - Format: `feature/phase-name-artifact` (e.g., `feature/phase03-user-stories`).
2. **Drafting:** Use the standard templates located in the `/templates/` directory when creating new core documents like BRDs or Use Cases.
3. **Review (PR):** Submit a Pull Request. Another analyst or the Project Sponsor must review the PR to ensure alignment with the Business Rules and Scope.
4. **Merge:** Squash and merge commits to keep the main history clean.

## 4. Formatting Standards
- **Markdown:** Use GitHub Flavored Markdown (GFM). Ensure all tables are properly aligned and headers use standard `#`, `##`, `###` hierarchies.
- **PlantUML:** Use standard `@startuml` and `@enduml` tags. Keep styling minimal and focus on logic.

## 5. Artifact Linking
Always use relative paths when referencing another document within the repository.
*Correct:* `[See BRD](../03_Requirements_Engineering/03_Business_Requirements_Document_BRD.md)`
*Incorrect:* `[See BRD](C:/Users/...)`
