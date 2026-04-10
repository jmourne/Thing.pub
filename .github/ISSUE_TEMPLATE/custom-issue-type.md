---
name: Custom Issue Type
about: Basic template for any component based issue
title: "[ Component ] Feature Name"
labels: ''
assignees: ''

---

### Goal
A concise description of the user benefit.

### Technical Requirements
Database: Specify schema (api) and any new tables or columns.
Logic: Describe the Rust backend expectations (e.g., "Function must accept UUID").
Security: List the specific RLS logic needed (e.g., "Author-only SELECT").

### Definition of Done
[ ] Code merged to main.
[ ] RLS policies verified in Supabase.
[ ] Security Advisor shows 0 warnings for these entities.
[ ] Relevant Wiki page updated.
