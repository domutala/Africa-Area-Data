# Organizational Structure – Africa Area Data

This document describes the organization of the **Africa Area Data** project and the roles of contributors to ensure data quality and consistency.

---

## 1. Division by Geographic Zone

The project is organized by **geographic zones**, each zone representing a country or a group of countries.  
Each zone has:  
- **A Zone Lead**: oversees data collection and validation, recruits contributors.  
- **Contributors**: add or correct data for the assigned zone.  
- **A validation process**: all contributions are reviewed by the zone lead before being integrated.

### Example Zones
- **West Africa**: Senegal, Mali, Côte d’Ivoire, etc.  
- **East Africa**: Kenya, Tanzania, Uganda, etc.  
- **Central Africa**  
- **North Africa**  
- **Southern Africa**

---

## 2. Roles and Responsibilities

### Zone Lead
- Recruit reliable contributors for their zone.  
- Review and approve **pull requests** or contributions for the zone.  
- Ensure data follows the **standard JSON structure** and quality guidelines.  
- Document the sources used for each contribution.  
- Serve as the point of contact for any questions regarding the zone.

### Contributors
- Add or correct data for their assigned zone.  
- Follow the **JSON structure** and maintain data quality.  
- Provide **sources and references** for each modification.  
- Participate in discussions and suggest improvements.

---

## 3. Contribution Workflow

1. **New contribution**: a contributor proposes an addition or modification for their zone.  
2. **Review by Zone Lead**: check JSON structure, data quality, and sources.  
3. **Validation and Integration**: once approved, the contribution is merged into the main database.  
4. **Documentation**: all sources and modifications are documented in the commit or in `sources.md`.

---

## 4. Advantages

- Clear distribution of responsibility and workload.  
- Quality control maintained through Zone Leads.  
- The project can **scale quickly** by recruiting new contributors.  
- Each zone becomes autonomous while adhering to a common structure across the project.
