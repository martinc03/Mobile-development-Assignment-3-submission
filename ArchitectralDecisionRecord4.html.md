Decision Title: Permission handling

Date: October 9 2023

Status: Approved

Context: The university requires a permissions system to control access to different parts of the application based on user roles (students, professors, administrators). The system will ensure that only authorized users can access and modify specific data while using the app.

Options:

* Access Control Lists (ACL)
* Attribute-based access control (ABAC)
* Role-Based Access Control (RBAC)

Decision: We chose to implement an Attribute-Based access control (ABAC)

Rationale: The reason we chose ABAC is due to its Granular access control which is something that the other permissions systems don't have. This allows for more precise control over user access rights based on specific attributes which is perfect for this app with its importance in protecting sensitive information. The school's database would work well with this permissions system as administrators could easily distribute permission constraints accordingly.

ACL and RBAC use a more simplistic system which would improve its performance, but we had to consider the features that would be implemented. The grading feature for example would benefit from ABAC's granular access control to avoid possible issues such as cheating.

Consequences:

* Slower Performance: Due to its granular access control, the system needing to process a large number of attributes and then having it be performed would hinder the app's performance.

Follow Up actions:

* Begin listing down possible constraints based on the school database
* Consider how to minimize performance issues
* Consider how users such as administrators would use this to add constraints to its staff and students
