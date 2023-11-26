Intent Filters:
1. Three Criteria for an Activity's Intent Filter:

Action: Describes the action to be performed (e.g., VIEW, EDIT, SEND).
Data: Specifies the data type the activity can work with (e.g., a specific MIME type or a URI pattern).
Category: Indicates additional information about the component (e.g., LAUNCHER, DEFAULT).
2. Retrieving the Intent:

An activity can retrieve the Intent that started it by calling getIntent() method.
3. Explaining Intents to a Non-Technical Friend:

Intents are like messages that different parts of an Android app can use to communicate. Imagine you have a friend who wants to share a photo with you. The friend puts the photo in an envelope, writes what they want you to do with it on the outside (like "look at this" or "edit this"), and adds any special notes. The envelope is then sent to you, and you follow the instructions on the outside.
Implicit vs. Explicit Intents:
1. Implicit Intents:

Usage: When you want the system to find an appropriate activity to handle the request.
Example: Opening a URL without specifying a particular browser.
2. Explicit Intents:

Usage: When you specify the exact activity to be invoked.
Example: Opening a specific screen in your app by specifying its class name.
3. Primary Information in an Intent:

Action: What to do (e.g., ACTION_VIEW).
Data: The data to act upon.
Category: Additional information or requirements for the component.