Where in your application should you check the current auth session?

The current auth session should be checked whenever you need to access user-specific information or perform actions that require user authentication. This includes tasks such as:

Displaying user profile information
Accessing user-specific data
Performing actions on behalf of the user (e.g., creating a post, submitting a form)
What is the command that is used to push your changes to the cloud?

The command that is used to push your changes to the cloud depends on the specific Amplify category you are working with. However, the general syntax is as follows:

amplify push <category>
Where <category> is the name of the Amplify category, such as auth, storage, or api. For example, to push your Auth configuration changes to the cloud, you would run the following command:

amplify push auth
What does Amplify Auth do for your application?

Amplify Auth provides a simple and secure way to manage user authentication and authorization in your application. It integrates with Amazon Cognito, a robust user directory service that handles user registration, authentication, account recovery, and other operations. Amplify Auth also provides a number of features that make it easy to add authentication to your application, such as:

Sign-in and sign-up workflows
Password reset and forgot password
Social authentication
User management