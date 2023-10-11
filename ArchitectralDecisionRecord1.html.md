Decision Title: Selection of Database Management System

Date: October 9 2023

Status: Approved

Context: Needed Database management that can utilize the university's existing active directory system to save the university data regarding its students, professors, classes, events and clubs.

Options:

* MY SQL
* PostgreSQL
* SQLite

Decision: We chose MySQL as our primary database management system due to its reliability, and data integrity.

Rationale: MySQL can support existing databases which would mean that the university's database would integrate properly with the application. MySQL is also well known for its data privacy and security which is perfect for the app as it can protect sensitive information. MySQL offers data encryption, user authentication authorization and access control. The app can only be used by users attending the university therefore databases that can provide protection for its data should be prioritized

MY SQL and PostgreSQL are also good options for databases due to their simplicity, performance and simplicity however MySQL was chosen due to its security features that would be more beneficial for this specific app. Its access control method makes it a more viable option.

Consequences:

* Performance issues: The application would be used heavily by professors and students which would decrease its performance leading to slower query responses.
* Possibility of data leaks: If access controls are not implemented correctly there's a possibility for sensitive information to not only be leaked but changed.
* Backup and Restore: The application with higher traffic would make it harder to back up the data.
* Database maintenance: The database would need to be maintained as the data can

Follow Up actions:

* Begin converting the university database into MySQL
* Consider how mySQL can be implemented into the application
* Consider how the user would interact with the app to access and alter data in the database
