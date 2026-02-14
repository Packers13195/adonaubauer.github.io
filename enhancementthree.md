<div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; font-weight: bold; margin-bottom: 20px;">
  <a href="https://packers13195.github.io/adonaubauer.github.io/">Home</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/capstonecourseinfo">Capstone Course Info</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/codereview">CodeReview</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/capstonecourseinfo/enhancementone">EnhancementOne</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/capstonecourseinfo/enhancementtwo">EnhancementTwo</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/capstonecourseinfo/enhancementthree">EnhancementThree</a> | 
  <a href="https://packers13195.github.io/adonaubauer.github.io/capstonecourseinfo/conclusion">Conclusion</a>
</div>

# Enhancement Three Details and Reflection
The third enhancement covers the database course area, and I decided that refactoring the inventory app that originally used a local sqlite database would fit this. I continued to build off my previous two enhancements for this third one as well. I began by setting up the new database which is Firebase. Firebase is a cloud-based database that offers more features and integration within a project than I could do with sqlite. 

To utilize Firebase, I set up FirebaseAuth which is for authorization to control the login and registration of users in the app. I found that FirebaseAuth can provide a default login and registration user interface. I refactored my project to use the FirebaseAuth user interface which could now control the login and registration of users to the inventory app. In the Firebase console I could manage some different variables with FirebaseAuth like enabling certain login methods. The sign-in method I chose is email/password, which allows users to create their own email and password credentials. There are other sign-in methods available, but I just implemented one method rather than overcomplicate it to allow other methods. Another feature is that I could set the password requirements so that Firebase could handle the validation of passwords when registering. The password requirements provide the security that is required for a user to register and login. 

The other feature of Firebase I used is Firestore Database. This database is a noSQL type database that holds data in a json collection. I refactored the user and item models in my project code to be able to use Firestore database. For the users collection I needed to save data for lastLoginTime, role, userEmail, and userId. The lastLoginTime is used when the user is trying to login. The role allows different features to be available, as I set roles for admin, user, and read-only. The userEmail and userId just hold the user information. 

The user collection was useful to implement role-based features. I implemented a read-only role which removed add item, edit item, and delete item options. Read-only users can only view the inventory on the inventory screen. I allow the user role to add and edit items, but they cannot delete items. The admin role is able to add, edit, and delete items. I also made a new feature for admins to view user management which allows them to change user roles for other users. Lastly, for visualization of the user logged in and their role, I added the user email and role into the appbar popup menu so users could see that they are logged in and what role they have.

I also set up the item collection which just holds the itemName and itemQuantity values. The item inventory screen still could utilize the list of items when getting the data from the firestore collection. There was only some minor refactoring of the code to get the data and display it.

This last enhancement completes outcomes two, four, and five. For outcome two I have well documented code so that anyone reviewing it understands what is being done. Outcome four I demonstrate the use of Firebase in my app with both using FirebaseAuth for registration and login management and using Firestore to hold user and item collections. FirebaseAuth also provides the security necessary to handle password hashing and input validation for login and registration keeping security in mind. Security is important for everything we do as software developers and is part of what builds a strong reputation for professional development as employers are looking for security driven individuals to protect their data.

Link to GitHub repository - [EnhancementThreeRepository](https://github.com/Packers13195/CS360-Mobile-Architecture-and-Programming)
