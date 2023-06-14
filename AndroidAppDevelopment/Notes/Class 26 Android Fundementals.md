## Reading

[Android fundamentals](https://developer.android.com/guide/components/fundamentals)

## Questions

1.  What is an Intent in Android Studios? Give some fresh examples of when you might use it.
	1. an Intent is used to start activites, services and broadcast recievers.
2.  Describe an Activity in your own word.
	1. an activity is a single screen with a user interface, such as your home screen on your phone or the interface that shows when your camera is open.

4.  Android App Development:

-   Android apps can be written using Kotlin, Java, and C++ languages.
-   Android SDK tools compile code, data, and resource files into an APK or an Android App Bundle.
-   APK is an archive file containing app contents required at runtime.
-   AAB is an archive file containing the entire project and additional metadata.
-   Google Play's servers generate optimized APKs based on the requesting device.

5.  Android App Security:

-   Each app runs in its own security sandbox.
-   Every app has a unique Linux user ID assigned by the system.
-   Apps run in their own processes with their own virtual machine (VM).
-   Apps have access only to the components and permissions granted to them.

6.  App Components:

-   Activities: Entry point for user interaction, representing a single screen.
-   Services: Run in the background to perform long-running operations or work for remote processes.
-   Broadcast receivers: Deliver system-wide broadcast events to the app, even when not running.
-   Content providers: Manage shared app data accessible by other apps.

7.  Component Activation:

-   Intents activate activities, services, and broadcast receivers.
-   Explicit intents specify a specific component, while implicit intents specify a component type.
-   Content providers are activated through the ContentResolver.

8.  Manifest File:

-   The manifest file (AndroidManifest.xml) declares app components.
-   It identifies required permissions, minimum API level, and hardware/software features.
-   It plays a crucial role in app installation and configuration.