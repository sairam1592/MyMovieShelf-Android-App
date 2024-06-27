# Steps to Delete the User Account

Deleting a user account in the My Movie Shelf Android App involves removing the user's data from both the Firebase Firestore Database and the local Room Database. Here are the comprehensive steps to achieve this:

# 1. Navigate to the Account Deletion Section
Open the app and navigate to the settings or user profile section.
Locate the "Delete Account" option.

# 2. Confirm Account Deletion
Click on the "Delete Account" button.
A confirmation dialog will appear to ensure the user wants to proceed with the account deletion. This dialog should explain that all data will be permanently removed.
Choose "Confirm" to proceed with deletion or "Cancel" to abort the process.

# 3. Backend Processing

Delete from Firebase Firestore:

The app will initiate a request to delete the user's document from the Firebase Firestore Database.
This will remove all data associated with the user's account stored in Firestore.
Delete from Room Database:

Concurrently, the app will initiate a request to delete the user's data from the local Room Database.
This ensures that no user data remains on the local device.

# 4. Feedback to User
After successfully deleting the account from both databases, the app should notify the user that their account has been deleted.
Redirect the user to the login or signup screen, as they are no longer authenticated.

# 5. Handling Errors
If there is an error during the deletion process, the app should notify the user with an appropriate error message.
Provide options to retry the deletion process or contact support for further assistance.

# Summary
Step 1: Navigate to the settings/profile section and locate the "Delete Account" button.
Step 2: Confirm the deletion through a confirmation dialog.
Step 3: The app will delete the user's data from Firebase Firestore and the local Room Database.
Step 4: Notify the user of successful deletion and redirect them to the appropriate screen.
Step 5: Handle any errors by providing retry options or support contact information.
This process ensures that the user's data is thoroughly removed from both remote and local storage, maintaining the integrity and privacy of the user's information.
