Decision Title: The Selection of a Caching Mechanism

Date: October 10 2023

Status: Approved

Context: The application needs to be optimized for low-end devices. There needs to be a caching mechanism to minimize data usage and allow for the low-end devices to run at the same performance as their higher-end model counterparts.

Options considered:

* Redis Cache
* In-memory caching
* Memcached

Decision: We have decided to implement an in-memory caching mechanism due to its efficiency.

Rationale: In-memory caching fetches data from the system's main memory rather than from its original data source. The app's users would be the university professors and students, their data would be protected which would mean that it would need to be decapsulated every time the user would use the app which would further increase the transmission time. Having the data be saved into the user's device would lessen the transmission time therefore increasing the app's performance. The app would need offline support, this form of data optimization would make this possible as the user's data would be saved to their device.

Out of all the options we chose in-memory caching is the better option as it fits more in line with the stakeholder's requirements of prioritizing data security. Memcached and Redis Cache are beneficial on their own, however. Memecached distributes its cached data to increase performance and Redis can cache queries. However, after evaluating its benefits in-memory caching is still the better option as the benefits from the other caching mechanisms aren't as necessary considering its smallish scope and In-memory caching would still offer the same amount of scalability and performance regardless.

Consequences:

* Limited Cache Size: In-memory caches are constrained by the available physical RAM from the user's device resulting in cache eviction and reduced cache hit rates.
* Constant Maintenance: The app allows users to check scheduling information and information regarding the user's grades and assignments. This data would need to be constantly updated as the data stored in the system would become outdated.
* App start time: This form of optimization would lead to an increased start time. The

Follow Up actions:

* Consider how the app would implement the caching mechanism
* Consider which data would be saved into the user's device
* Consider how the cached data could be updated
