[Amplify and Cognito](https://docs.amplify.aws/lib/auth/getting-started/q/platform/android/) (read “Getting started” and “Sign in” subsections)

1. Where in your application should you check the current auth session?
	1. For testing purposes, you can run this from your MainActivity's `onCreate` method.
		1. Amplify.Auth.fetchAuthSession( result -> Log.i("AmplifyQuickstart", result.toString()), error -> Log.e("AmplifyQuickstart", error.toString()) );
2. what is the command that is used to push your changes to the cloud?
	1.  amplify push
3. What does Amplify Auth do for your application?
	1. adds authentication to your app