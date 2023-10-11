Decision Title: Mobile App Architecture for Social Media Platform

Date: October 9 2023

Status: Approved

Context: We need to define the architectural structure for our mobile application to ensure maintainability and optimal performance.

Options considered:

* Microservice
* Abstract factory pattern
* Adapter pattern

Decision: We will use the scalable architecture based on the Model-View-Model (MVVM) design pattern. It is the most common design pattern for mobile app development and is key to building a scalable and maintainable app.

Rationale: MVVM separates its UI components and back-end code which would make it easy considering the complexity of the app. It's also good for long-term development as the separation would make it easier to test and update the app. The app would also have a lot of features, most notably its accessibility features. Developing an app based on this structure would make the process easier.

We chose not to do the following options as MVVM is the most simple and fitting one specifically for the mobile app. The microservice pattern is too complex as the features implemented aren't complex enough to warrant it. The abstract method is also a good option to help develop the interface of a social media app considering creating families of related objects would simplify the process however MVVM is better in terms of simplicity. The adapter pattern is the same way but its benefits of class integration aren't what's needed for a social media app.

Consequences:  

* Memory leaks: There's a possibility of memory leaks if subscriptions in the view model and references are implemented poorly
* Design Decision complexity: Based on the pattern structure of the app there is a possibility of code being repeated through various parts of the program as a structure for the program to function. Developing the program may become tedious, leading increasing the development time for the app

Follow Up actions:

* Draft low-fidelity sketches for how the app may look like
* Decide on the app's features and how they would be implemented in consideration of the low-fidelity sketches
* Decide on what framework and possible languages for the app's backend development
