Decision Title: UI Framework

Date: October 9, 2023

Status: Approved

Context: We need to select a UI framework for developing the university social networking app. The choice of UI framework is needed for the app's user interface and user experience.

Options:

* Native UI (Swift for iOS, Kotlin for Android)
* Web UI (React, Angular, or Vue.js)
* Hybrid UI (React Native or Flutter)

Decision: We have decided to use a hybrid approach and use React Native as our framework.

Rationale: React Native offers a balance between native performance and cross-platform development. It is good for creating a responsive and user-friendly interface for our app on both iOS and Android. React native also offers built-in and third-party libraries with features such as text-to-speech and other assistive technologies that will allow the app to be inclusive.

Web UI and Hybrid UI fall short in terms of performance which is the most important aspect for this UI. The UI should be fast and easy for its users, more so with university students and its staff where time is important for them. Native is also easier for developers to work with.

Consequences:

* Although react native allows for cross-platform development some features are unique to a certain platform (iOS and Android). This can increase development complexity.

Follow-Up Actions

* Start development using react native that meets requirements.
