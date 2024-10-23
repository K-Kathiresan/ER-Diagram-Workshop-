# ER-Diagram-Workshop:
## ER DIAGRAM(University Database):
![university dbbms drawio](https://github.com/user-attachments/assets/b81d3f69-305c-419b-8575-8eaa14771601)
Here’s the ER diagram based on university database scenario, including the entities, relationships, attributes, and cardinality/participation constraints. The diagram also incorporates the concept of course prerequisites.
## Design Choices and Explanation:
### Entities:
Program: Captures the different academic programs with unique Program_ID.
Department: Governs the academic programs.
Student: Contains student information like Admission_No, Full_Name, etc.
Course: Stores course details such as Course_No, Credits, etc.
Instructor: Holds information about teaching staff.
Enrollment: Captures student course registration details.
Prerequisite: Represents the relationships between courses and their prerequisites.
### Relationships:
Offers: Links Program and Course.
Registers: Connects Student with Enrollment, tracking which courses they are enrolled in.
Teaches: Connects Instructor with Course.
Has Prerequisite: Represents the relationship between courses where one course is a prerequisite for another.
## Concept of Prerequisites:
The Prerequisite relationship handles cases where certain courses require other courses to be completed first. For example, a student may need to complete "Intro to Programming" before enrolling in "Data Structures." This is represented as a 1 relationship, where a course can have multiple prerequisites, and each prerequisite can apply to multiple courses.
