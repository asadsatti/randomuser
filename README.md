# randomuser
App using Randomuser API

Smmary:

a) Your overall approach
-Each API call loads 30 user records asynchronously
-User Jackson to convert JSON for a use record to User object
-User objects are stored an ArrayList to be used as a data source for RecyclerView
-RecyclerView to display the list of users because RecyclerView requires to use ViewHolder pattern for better performance
-Chosen to display user name and phone only for each user
-Taping user's name converts the User object to JSON string and passes to user detail Activity 
-User detail Activity loads user's detail in a fragment
-User object to JSON string conversion is done because I haven’t implemented User as Parcelable which is needed in order to pass to another Activity
-User's photo is also downloaded asynchronously

b) What platform you chose and why you chose it

Development & Test environment:
-Android platform
-Android Studio IDE
-Test device Nexus 4 with Android Lollipop

c) What features you completed

-App loads users from the Randomuser API
-Each page request load 30 users
-Scrolling loads news user if number of users yet to be display is down to 10 for smooth scrolling
-Taping user loads user's profile
-Tested by scrolling be more than 45 pages

d) Given more time, what else would you have liked to complete and how long it would have taken you?

-Make UI pretty
-Make phone, email, and address actionalble fields
-Use nicer fonts
-Add animations
-Add splash screen
-Taping on the right side of list item doesn't work. It should be fixed

e) Given more time, what else would you have done to make the project more robust?

-Use  Picasso library to download images
-Use retrofit library
-Modify the API request to exclude the parameters from response that are not needed
-Test with two pan devices e.g., tablets
-Implement User class as Parcelable
