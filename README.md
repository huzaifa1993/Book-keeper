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

*showModal():<br>
 function is used to display a modal on the UI. It adds the 'show-modal' class to the modal element to make it visible and sets the focus on the website name input element.<br>
 this function called when the 'Add Bookmark' button is clicked. <br>
 -this function does not take any parameter.<br>
 -this function does returns void. <br>
 -this function is used to modify the Document Object Model (DOM).


*validate(nameValue,urlValue)<br>
 -This function is called to validate input data and check whether the URL is a valid web address or not.<br>
 it takes two parameters:<br>
 -nameValue: a string representing the name value.<br>
 -urlValue: a string representing the URL value.<br>
 This function returns a boolean value:<br>
 true: if both the fields have valid values and the URL provided is in the correct format.<br>
 false: if either of the fields is empty or the URL provided is not in the correct format.<br>
 -The function uses a regular expression to validate the URL. The regular expression matches the a specific pattern.<br>
 -The alert() function is used to display alert messages to the user.<br>


*buildBookmarks():<br>
 -This function is used to build and display a list of bookmarks on a web page.<br>
 -it takes no arguments and returns void.<br>
 -uses the global bookmarks array to get the data for calling bookmarks.<br>
 -Clear the bookmarks container.<br>
 -it loops through each bookmark in the bookmarks array using forEach.<br>
 -Create a new HTML element to display the bookmark item.<br>
 -Create a close icon for the bookmark item that allows the user to delete the bookmark.<br>
 -Create a div element to display the link information (name and favicon).<br>
 -Create an image element to display the favicon for the bookmark.<br>
 -Create an anchor element to display the name of the bookmark and set its target to _blank to open it in a new tab.<br>
 -Add the favicon and name to the link information div element.<br>
 -Add the close icon and link information div element to the bookmark item.<br>
 -Add the bookmark item to the bookmarks container.<br>


Functions:<br>
*fetchBookmarks():<br>
 -this function checks if there are any bookmarks in the browser's local storage. If there are no bookmarks in the local storage, it will add a default bookmark.<br>
 -This function does not take any parameter and returns an array of object of two properties:<br>
 .name: the title of the bookmark.<br>
 .url: the URL of the bookmark.<br>


*deleteBookmark(url):<br>
 -This function is used to delete a bookmark from the bookmarks array and from local storage. <br>
 -it takes a url as parameter.<br>
 -The function loops through each bookmark using the forEach method.<br>
 -If the URL of the current bookmark matches the url parameter, the splice method is used to remove that bookmark from the bookmarks array.<br>


*storeBookmark(e):<br>
 -this function adds a new bookmark to bookmarks array and updates the localStorage and and resets the form used to create the new bookmark.<br>
 -it takes 'e' as parameter.<br>
 -preventDefault method prevents the default behavior of the form submission.<br>
 -pulls the value of the website name and URL from the form input fields.<br>
 -it checks if the website name and URL are valid using the validate.<br>
 -If the validation succeeds, the function creates a new bookmark object with the website name and URL and adds it to the bookmarks array using the push method.<br>
 -it calls the fetchBookmarks function to update the displayed bookmarks list on the webpage.<br>
 -The form used to create the new bookmark is reset using the reset method.<br>
 -The focus is set on the website name input field using the focus method.