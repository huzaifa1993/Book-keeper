# Book-keeper
Book-Keeper Project: <br>
 is a simple  web application that allows users to save   their favourite websites in local storage.<br>
 Users can add and delete their bookmarks easily.

Getting Started:<br>
 To use Book-keeper Project, you will need to have a web browser installed on your computer or mobile device.<br> 
 The application is accessible through any web browser.

 Features:<br>
 -Add bookmarks: Users can add new bookmarks to the application by providing the website URL and title.<br>
 -Delete bookmarks: Users can delete bookmarks that are no longer needed.<br>
 -Responsive Design: The application is optimized for different screen sizes, including desktops, laptops, tablets, and smartphones.

Technologies Used:<br>
 HTML, CSS, JavaScript

Styling:<br>
 -Nunito font is used in this website and sans-serif font as default font.<br>
 -Flex box is used for the layout. <br>
 -SVG image as a background for the website.<br>

Functions:
*fetchBookmarks():
 -this function checks if there are any bookmarks in the browser's local storage. If there are no bookmarks in the local storage, it will add a default bookmark.
 -This function does not take any parameter and returns an array of object of two properties:
 .name: the title of the bookmark.
 .url: the URL of the bookmark.

*showModal():
 function is used to display a modal on the UI. It adds the 'show-modal' class to the modal element to make it visible and sets the focus on the website name input element.
 this function called when the 'Add Bookmark' button is clicked. 
 -this function does not take any parameter.
 -this function does not return any value. 
 -this function is used to modify the Document Object Model (DOM).