<head> <link href="/adonaubauer.github.io/assets/css/lightbox.css" rel="stylesheet" /></head>
{% include navigationmenu.html %}

# Enhancement Two Details and Reflection
Using the Inventory Warehouse app artifact from the CS360 Mobile Architecture and Programming course for this second enhancement is what I wanted to do. I built from the redeveloped Flutter app from enhancement one and focused on developing in the course area algorithms and structures. This area could be enhanced in the inventory app for the inventory item screen. I developed a search item by name, filtering options, and sorting options. To create these features, I got the data from the database and used the data structure of list.

To search for an item the app queries the SQLite database with the string entered in the search field once the user clicks the search button. The results of the query are returned as a list to be displayed on the screen to the user. Similarly, for the filtering the app will also query the database to find items with quantities greater than 5 and items with quantities less than or equal to 5. Lastly, for the sorting feature the app uses the list structures sort method to sort the items. The sort method is part of the flutter library, and it compares the objects to determine the order of the list and return it. The sorting function adjusts the list to ascending or descending order by item name. The sorting can also be done for item quantity from low to high and high to low. 

These features of search, sort, and filter fulfill a few outcomes. One outcome it completes is outcome three - Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices. This is completed with the user of the sort and compareTo methods to process the data. Another outcome it fulfills is outcome four - Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals. I utilize flutter and sqlite tools to implement the search, sort, and filter options which provide these basic features to the user. The user can easily adjust the inventory to show what they would like to see whether that be a specific item with the search criteria, or with options to filter out items that do not fit the filter criteria, or lastly to reorder items to see items by a-z or z-a order, or even by low to high and high to low quantities. I also completed outcomes one with the use of Git and Github to upload my project to the repository to make it available for collaboration, and outcome two with improved documentation within my code files to deliver professional oral, written, and visual communications.

Link to GitHub repository - [EnhancementTwoRepository](https://github.com/Packers13195/CS360-Mobile-Architecture-and-Programming/tree/algorithmsanddatastructuresenhancement/searchandfilterfeatures)

## Screenshots
<div class="gallery-container" style="display: flex; flex-wrap: wrap; gap: 20px;">
  
  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2iteminventorynoitems.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Inventory Screen">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2iteminventorynoitems.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Inventory Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Inventory Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2itemsearchresults.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Searching for Item">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2itemsearchresults.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Search Screen">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Search Screen</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2filteroptions.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Item Filters">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2filteroptions.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Filter Options">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Filter Options</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2itemslessthan5.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items less than 5 quantity Filter">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2itemslessthan5.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Less than 5 quantity filter">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Less than 5 quantity filter</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2itemsquantitymorethan5.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items more than 5 quantity Filter">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2itemsquantitymorethan5.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="More than 5 quantity filter">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">More than 5 quantity filter</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2sortingoptions.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items Sorting Options">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2sortingoptions.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Sorting Options">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Sorting Options</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2sortedatoz.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items Sorting A to Z">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2sortedatoz.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Sorting A to Z">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Sorting A to Z</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2sortedztoa.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items Sorting Z to A">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2sortedztoa.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Sorting Z to A">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Sorting Z to A</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2sortedlowtohighquantity.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items Sorting low to high quantity">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2sortedlowtohighquantity.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Sorting low to high quantity">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Sorting low to high quantity</p>
  </div>

  <div style="text-align: center; width: 200px;">
    <a href="{{ '/assets/images/enhancement2screenshots/enhancement2sortedhightolowquantity.png' | relative_url }}" 
       data-lightbox="enhancement2" 
       data-title="Enhancement Two: Items Sorting high to low quantity">
      <img src="{{ '/assets/images/enhancement2screenshots/enhancement2sortedhightolowquantity.png' | relative_url }}" 
           style="width: 100%; border-radius: 8px; border: 1px solid #ddd;" 
           alt="Item Sorting high to low quantity">
    </a>
    <p style="font-size: 0.9rem; margin-top: 8px; color: #555;">Item Sorting high to low quantity</p>
  </div>

</div>

<script src="/adonaubauer.github.io/assets/js/lightbox-plus-jquery.js"></script>
