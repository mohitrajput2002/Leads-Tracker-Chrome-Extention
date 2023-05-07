# Leads-Tracker-Chrome-Extention

![Screenshot (1355)](https://user-images.githubusercontent.com/67924939/236660346-f2fd3081-3595-4e83-97fa-ea3debca366d.png)

A Chrome extension called `"Leads Tracker"`. Based on the design, users can save tabs and links using this extension, and can also delete the saved links. 

To build this extension, you would need to use HTML, CSS, and JavaScript. Here are some general steps you can follow:

1. Set up the basic HTML structure for the extension popup. This will include a header, a section for displaying saved links, and a form for adding new links.
2. Use CSS to style the popup according to the design you have provided. This will include defining colors, fonts, and layout.
3. Write JavaScript code to handle user interactions with the extension. This will include adding event listeners to the form, saving and deleting links using Chrome's storage API, and updating the UI when links are added or deleted.

Here are some specific tips for implementing each feature:

Saving tabs:
- Use the `chrome.tabs` API to get information about the current tab and save it to storage.
- When the user clicks on a saved tab in the UI, use the `chrome.tabs` API to open that tab in a new window.

Saving links:
- Add an event listener to the form submit button to capture the link URL and save it to storage.
- When the user clicks on a saved link in the UI, use the `chrome.tabs` API to open that link in a new tab.

Deleting all links:
- Add a delete all button next to save tab button in the UI.
- Add an event listener to delete all button to remove the corresponding links from storage and update the UI.
