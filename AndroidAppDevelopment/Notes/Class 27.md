Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

## Reading

[Android SharedPreferences](https://developer.android.com/training/data-storage/shared-preferences)

[Espresso Testing (read Overview, Basics, and Recipes, plus any others that look interesting)](https://developer.android.com/training/testing/espresso)

-   Espresso is used for writing Android UI tests.
-   It promotes concise, beautiful, and reliable tests.
-   A code snippet example Java 
	- @Test public void greeterSaysHello()  { 
	
		onView(withId(R.id.name_field)).perform(typeText("Steve")); 
		
		onView(withId(R.id.greet_button)).perform(click()); 
		
		onView(withText("Hello Steve!")).check(matches(isDisplayed())); }
	
-   Espresso tests express expectations, interactions, and assertions clearly without boilerplate content or messy implementation details.
-   Espresso tests run optimally fast and handle UI manipulation and assertions efficiently.
-   Espresso provides synchronization capabilities to ensure reliable test results.
-   Synchronization conditions include checking the message queue, AsyncTask execution, and idling resources.
-   The espresso-core package contains core functionalities, while other packages provide additional resources and extensions.
-   Packages include espresso-web, espresso-idling-resource, espresso-contrib, espresso-intents, and espresso-remote.

[Ridiculous superpower: the Espresso Test Recorder](https://developer.android.com/studio/test/espresso-test-recorder)

[Android Tasks and the Back Stack](https://developer.android.com/guide/components/activities/tasks-and-back-stack)

## Questions

1.  What is a technology you’ve used before that is similar to Shared Preferences?
2.  Why is testing important? Give at least 4 reasons, and explain which is the most important to you and why.
	1. 1.  Bug detection and prevention: Testing helps identify and address software defects early in the development process, reducing the risk of critical errors in production.
    
2.  Reliability and stability: Testing ensures that software performs as expected and delivers reliable functionality, maintaining a positive user experience.
    
3.  Software quality improvement: Testing enhances the overall quality of software by verifying requirements, optimizing performance, and improving user satisfaction.
    
4.  Code refactoring and maintainability: Testing facilitates code refactoring and maintains the software's quality over time, making it easier to maintain and update.
    

The most important reason for me personally is bug detection and prevention. Early detection of bugs can save significant time and resources by addressing issues before they become more complex and costly to fix. It also helps in delivering a more reliable and stable product to users, which is crucial for building trust and ensuring a positive user experience.

3.  Create an analogy for Tasks and the back stack. Have we used a similar system before? Explain.
	1. This could be compared to a stack of dishes, this is similar to the call stack that weve worked with before.