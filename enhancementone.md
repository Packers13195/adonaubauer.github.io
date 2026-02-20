<head> <link href="/adonaubauer.github.io/assets/css/lightbox.css" rel="stylesheet" /></head>
{% include navigationmenu.html %}

# Enhancement One Details and Reflection
The artifact I selected after reviewing several projects across my educational journey was the Inventory Warehouse app which I developed in the CS360 Mobile Architecture and Programming course at Southern New Hampshire University. The app was a simple android app that allows the user to register an account, login with that account, then view inventory items, edit or delete those items, add items to a SQLite database, and it included a push notification to alert users to low quantity items. I chose this artifact due to my history and knowledge of mobile applications from my associate degree program that I completed. I am most confident in my skills and abilities in this area of computer science and felt most confident in showing this project and the enhancement of it in my ePortolio. Since the original artifact was written in java and xml, the first enhancement I planned is to use the Flutter framework and redevelop the artifact in dart language. This shows my skills in mobile application development and understanding how to utilize the Flutter framework to create a cross-platform app that can be run on both android and iOS.

Flutter is an industry standard tool that I hope to use more in both my continuing education and in a professional setting. I made minor changes from the original project throughout development of this enhancement, such as changes to the home screen buttons and bottom navigation buttons. I also improved the UI of the inventory screen to display the items a bit differently. Lastly, I improved the validation of both the add item screen and the user registration forms and added hashing to the password, so the raw password is no longer saved in the database. 

In this enhancement, I completed the planned outcome about designing and developing a solution to solve a problem, as now with the redevelopment of the app in Flutter, it has become a cross-platform app that can run on both android and iOS. Another outcome completed is the security outcome, since I was able to implement better form validation and hashing the password. Another outcome it covers is the use of an industry standard tool like Flutter. I enjoyed the process of revisiting the original artifact and was able to work through each element to implement them in Flutter. I made small changes compared to the original which I feel makes the new app more secure such as hashing the password instead of saving the raw password.

Dart is the coding language used to develop in the Flutter framework, so I reviewed a lot of the documentation for the different libraries to learn how to develop my app. In enhancement two and enhancement three, I will be working with this same artifact to build off of this first enhancement. This will give me more opportunities to continue using Flutter and get more experience with it.

Link to GitHub repository - [EnhancementOneRepository](https://github.com/Packers13195/CS360-Mobile-Architecture-and-Programming/tree/softwareengineeringanddesignenhancement/flutter-rebuild)

## Screenshots
<div class="gallery-container" style="display: flex; flex-wrap: wrap; gap: 20px;">
  
  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1loginscreen.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Custom Login Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1loginscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Login Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Login Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1registrationscreen.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Custom Registration Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1registrationscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Registration Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Registration Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1homescreen.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: User Home Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1homescreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Home Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Home Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1inventoryscreennoitems.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Inventory Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1inventoryscreennoitems.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Inventory Screen with no items Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Inventory Screen with no items</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1inventoryscreenwithitems.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Inventory Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1inventoryscreenwithitems.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Inventory Screen with items Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Inventory Screen with items</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1additemscreen.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Add Item Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1additemscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Add Item Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Add Item Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement1screenshots/enhancement1edititemscreen.png' | relative_url }}" 
       data-lightbox="enhancement1" 
       data-title="Enhancement One: Edit Item Screen">
      <img src="{{ '/assets/images/enhancement1screenshots/enhancement1edititemscreen.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Edit Item Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Edit Item Screen</p>
  </div>

</div>

<script src="/adonaubauer.github.io/assets/js/lightbox-plus-jquery.js"></script>
