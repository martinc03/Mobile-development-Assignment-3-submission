Decision Title: Backend Language

Date: October 9, 2023

Status: Approved

Context: We need to choose a backend programming language for the university social networking app. The backend language is useful in handling server-side logic and data management.

Options:

* Python
* Java
* Node.js

Decision: We have decided to use Node.js as the backend language for the university social networking app.

Rationale: Node.js uses JavaScript which will allow for simpler development because the languages are consistent on both the backend and frontend. Node can also interact with push notification services such as Firebase Cloud Messaging and with node being scalable, it will help the performance of accessing real-time push notification services.

Node is beneficial compared to its other options due to its overall performance. Python executes one process at a time while Java has a higher chance of error due to the amount of lines in a code.

Consequences:

* Node.js relies heavily on asynchronous code and callbacks. Managing asynchronous code can lead to problems if not structured well. Techniques such as async/await can be used to manage asynchronous code.

Follow-Up Actions:

* Start development with Node.js
