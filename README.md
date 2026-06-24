# Student-course-enrollment-system
A console-based Course Registration System built in **C++** using core Data Structures concepts. The system manages students, courses, enrollments, and waitlists through an interactive menu-driven interface.

---

## Data Structures Used

| Structure | Purpose |
|---|---|
| Linked List | Storing and traversing student records |
| AVL Tree | Storing and searching courses efficiently (O log n) |
| Max Heap | Managing waitlist priority based on student GPA |
| Stack | Undo and Redo functionality for enrollment actions |

---

## Features

- **Student Management** — Register students with ID, name, and department validation
- **Course Management** — Add courses with capacity limits and department assignment
- **Enrollment System** — Enroll students in courses with prerequisite and department checks
- **Waitlist System** — Automatically adds students to a GPA-priority waitlist when a course is full; promotes highest GPA student when a seat opens
- **Prerequisite Handling** — Add prerequisites to courses with cycle detection to prevent circular dependencies
- **Undo / Redo** — Reverse or reapply the last enrollment or drop action using stacks
- **Search & Filter** — Search students by ID or department; search courses by ID or department
- **GPA Management** — Update student GPA; GPA affects waitlist priority
- **Persistent Storage** — Data saved and loaded from binary files (`students.dat`, `courses.dat`); human-readable text files also generated (students.txt, courses.txt)

---

## Constraints

- Max students: 1000
- Max courses: 100
- Max courses per student: 10
- Max students per course: 100
- Max prerequisites per course: 5
- Max waitlist size per course: 100

---

## Technical Stack

* **Language:** C++
* **Core Focus:** Data Structures & Algorithms
* **Data Structures Used:**
    * **AVL Trees:** Balanced course storage for $O(\log n)$ search time.
    * **Max-Heaps:** Priority waitlist management.
    * **Stacks:** Undo/Redo system history tracking.
    * **Linked Lists:** Student records and enrollment links.
* **Concepts Applied:**
    * Tree rotations (LL, RR, LR, RL)
    * Heap operations (Insert, Extract-Max)
    * Graph traversal (Cycle Detection)

## Contributors

* **Noor Fatima (Leader)** – Core structures, file handling, prerequisite logic, debugging
* **Adnan Haider** – AVL tree implementation, undo/redo stacks, CLI system
* **Areeba Kanwal** – Enrollment logic, heap-based waitlist, capacity handling
* **Musfirah Imran** – Student management, search features, GPA updates

## Future Improvements

* **GUI-based system:** Transition to a desktop or web interface.
* **Role-based access:** Separate dashboards for Admin and Student views.
* **Automatic timetable conflict detection:** Prevent overlapping schedules.
* **CSV import/export support:** For easier bulk data management.
* **Timetable Conflict Detection:** Prevent students from enrolling in courses that have overlapping schedules.

---
**Developed for Semester Project – COMSATS University Islamabad**


