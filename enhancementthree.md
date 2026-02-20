<head> <link href="/adonaubauer.github.io/assets/css/lightbox.css" rel="stylesheet" /></head>
{% include navigationmenu.html %}

# Enhancement Three Details and Reflection
The third enhancement covers the database course area, and I decided that refactoring the inventory app that originally used a local sqlite database would fit this. I continued to build off my previous two enhancements for this third one as well. I began by setting up the new database which is Firebase. Firebase is a cloud-based database that offers more features and integration within a project than I could do with sqlite. 

To utilize Firebase, I set up FirebaseAuth which is for authorization to control the login and registration of users in the app. I found that FirebaseAuth can provide a default login and registration user interface. I refactored my project to use the FirebaseAuth user interface which could now control the login and registration of users to the inventory app. In the Firebase console I could manage some different variables with FirebaseAuth like enabling certain login methods. The sign-in method I chose is email/password, which allows users to create their own email and password credentials. There are other sign-in methods available, but I just implemented one method rather than overcomplicate it to allow other methods. Another feature is that I could set the password requirements so that Firebase could handle the validation of passwords when registering. The password requirements provide the security that is required for a user to register and login. 

The other feature of Firebase I used is Firestore Database. This database is a noSQL type database that holds data in a json collection. I refactored the user and item models in my project code to be able to use Firestore database. For the users collection I needed to save data for lastLoginTime, role, userEmail, and userId. The lastLoginTime is used when the user is trying to login. The role allows different features to be available, as I set roles for admin, user, and read-only. The userEmail and userId just hold the user information. 

The user collection was useful to implement role-based features. I implemented a read-only role which removed add item, edit item, and delete item options. Read-only users can only view the inventory on the inventory screen. I allow the user role to add and edit items, but they cannot delete items. The admin role is able to add, edit, and delete items. I also made a new feature for admins to view user management which allows them to change user roles for other users. Lastly, for visualization of the user logged in and their role, I added the user email and role into the appbar popup menu so users could see that they are logged in and what role they have.

I also set up the item collection which just holds the itemName and itemQuantity values. The item inventory screen still could utilize the list of items when getting the data from the firestore collection. There was only some minor refactoring of the code to get the data and display it.

This last enhancement completes outcomes two, four, and five. For outcome two I have well documented code so that anyone reviewing it understands what is being done. Outcome four I demonstrate the use of Firebase in my app with both using FirebaseAuth for registration and login management and using Firestore to hold user and item collections. FirebaseAuth also provides the security necessary to handle password hashing and input validation for login and registration keeping security in mind. Security is important for everything we do as software developers and is part of what builds a strong reputation for professional development as employers are looking for security driven individuals to protect their data.

Link to GitHub repository - [EnhancementThreeRepository](https://github.com/Packers13195/CS360-Mobile-Architecture-and-Programming/tree/databases/firebasemigration)

## Screenshots
<div class="gallery-container" style="display: flex; flex-wrap: wrap; gap: 20px;">
  
  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3loginscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: FirebaseAuth Login Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3loginscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="FirebaseAuth Login Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">FirebaseAuth Login Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3registrationscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: FirebaseAuth Registration Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3registrationscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="FirebaseAuth Registration Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">FirebaseAuth Registration Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3adminuserhomescreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Admin Home Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3adminuserhomescreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Admin Home Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Admin Home Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3adminmenuoptions.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Admin User Menu Options">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3adminmenuoptions.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Admin User Menu Options">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Admin Menu Options</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3adminusermanagementscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Admin User Management Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3adminusermanagementscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Admin User Management Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Admin User Manage Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3adminroleinventoryscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Admin Inventory Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3adminroleinventoryscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Admin Inventory Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Admin Inventory Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3userrolehomescreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: User Home Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3userrolehomescreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="User Home Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">User Home Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3useriteminventoryscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: User Inventory Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3useriteminventoryscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="User Inventory Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">User Inventory Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3readonlyrolehomescreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Read Only User Home Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3readonlyrolehomescreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Read Only User Home Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Read Only User Home Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement3screenshots/enhancement3readonlyroleinventoryscreen.png' | relative_url }}" 
       data-lightbox="enhancement3" 
       data-title="Enhancement Three: Read Only User Inventory Screen">
      <img src="{{ '/assets/images/enhancement3screenshots/enhancement3readonlyroleinventoryscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Read Only User Inventory Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Read Only User Inventory Screen</p>
  </div>

</div>

<script src="/adonaubauer.github.io/assets/js/lightbox-plus-jquery.js"></script>
