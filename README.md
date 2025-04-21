Library Project

This is a simple JavaScript library app where you can add books, display them, remove them, and update their read status. It's a beginner project focused on learning constructors, DOM manipulation, and separating data from display logic.

 How It Works

All books are stored in an array called myLibrary.

Each book is created using a Book constructor function.

The addBookToLibrary() function creates a new book and pushes it to the array.

Each book has a unique ID generated with crypto.randomUUID() to keep track of it, even when books are removed or reordered.

 Features

Add Book: Click the "New Book" button to open a form. Fill in the details (title, author, pages, read status) and submit.

Display Books: Books are shown on the page (cards or table style). Each one displays the book’s details.

Remove Book: Each book has a "Remove" button that deletes it from the library and updates the display.

Toggle Read Status: Each book also has a "Toggle Read" button. This uses a prototype function on the Book object to change the read status.

Displaying Books

A function called renderBooks() loops through myLibrary and creates elements in the DOM for each book.

Each book element includes:

Title, author, pages, read status

A Remove button

A Toggle Read button

The buttons use data-id attributes to connect the DOM to the book object by ID.

 Form Submission

The "New Book" form uses event.preventDefault() to stop the page from refreshing when submitted.

After submitting, a new book is added and the display updates automatically.