# Entity-Relationship (ER) Modeling

## 1. Guided Example: University Registration System
A conceptual database design for university course registration and department management.
**Key Entities:** Student, Course, Lecturer, Department[cite: 2].

### ER Diagram
![University ERD](./assets/university-system.svg)

### Key Relationships & Constraints
| Relationship | Participating Entities | Cardinality | Justification |
| :--- | :--- | :--- | :--- |
| **Register** | Student – Course | M:N | A student can register for multiple courses, and a course can have multiple students enrolled[cite: 2]. |
| **Teach** | Lecturer – Course | 1:N | A lecturer teaches multiple courses, but each course is taught by exactly one lecturer[cite: 2]. |
| **Offer** | Department – Course | 1:N | A department offers multiple courses, but each course is offered by exactly one department[cite: 2]. |
| **Belong** | Lecturer – Department | 1:N | A lecturer belongs to exactly one department, while a department has multiple lecturers[cite: 2]. |

---

## 2. Case Study: Clinic Management System
A database design for a clinic management system[cite: 1].
**Key Entities:** Patient, Doctor, Treatment, Consultation, Appointment, Department[cite: 1].

### ER Diagram
![Clinic ERD](./assets/clinic-system.svg)

### Key Relationships & Constraints
| Relationship | Participating Entities | Cardinality | Justification |
| :--- | :--- | :--- | :--- |
| **WorksIn** | Doctor – Department | N:1 | Every doctor works in exactly one department (Total participation on Doctor, Partial on Department)[cite: 1]. |
| **Produces** | Appointment – Consultation | 1:1 | Each appointment produces exactly one consultation record[cite: 1]. A consultation record cannot exist without its appointment (Identifying relationship)[cite: 1]. |

---

## 3. Case Study: Library Management System
A database design for a small library system[cite: 3].
**Key Entities:** Title, Copy (Weak Entity), Member[cite: 3].

### ER Diagram
![Library ERD](./assets/library-system.svg)