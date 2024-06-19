# Library Management System

Welcome to the Library Management System project! This is a simple command-line application designed to manage a collection of books using Object-Oriented Programming (OOP) principles in TypeScript.

## Objectives

- **Implement OOP Principles:** Demonstrate the use of classes, interfaces, and methods in TypeScript.
- **Create a Simple CLI Application:** Use the `inquirer` library to create an interactive command-line interface.
- **Manage a Collection of Books:** Allow users to add, find, and list books in a library.

## Features

### 1. Add Book
Allows users to add a new book to the library by entering the title and author of the book.

### 2. Find Book (with partial match)
Enables users to search for a `book` by its `title` or `author` and displays the book details if found. **The search feature supports partial matches, meaning you can find a book by entering part of the title or the author's name.**

### 3. List Books
Displays a list of all the books currently available in the library.

### 4. Exit
Exits the application.

## Definitions

- **Interface:** A structure that defines the contract in your application. In this project, the `Book` interface defines the structure of a book object.
- **Class:** A blueprint for creating objects. The `Library` class in this project manages the collection of books.
- **Method:** A function associated with an object. Methods in the `Library` class include `addBook`, `findBooks`, and `listBooks`.

## Installation

To run this project, you need to have [Node.js](https://nodejs.org/) installed on your system. Then, follow these steps:

1. Clone this repository:
    ```sh
    git clone https://github.com/your-username/library-management-system.git
    ```
2. Navigate to the project directory:
    ```sh
    cd library-management-system
    ```
3. Install the dependencies:
    ```sh
    npm install
    ```
4. Run the application:
    ```sh
    npm start
    ```

## Usage

Once the application is running, you will be prompted with a menu where you can choose one of the following actions:

- **Add Book:** Enter the title and author to add a new book to the library.
- **Find Book:** Enter the title or author to search for a book in the library.
- **List Books:** Display all books currently in the library.
- **Exit:** Close the application.

### Example

#### Adding a Book

1. Select `Add Book` from the menu.
2. Enter the book title and author when prompted.

    ```plaintext
    ? What would you like to do? (Use arrow keys)
    ❯ Add Book 
      Find Book 
      List Books 
      Exit 
    ? Enter the book title: The Great Gatsby
    ? Enter the book author: F. Scott Fitzgerald
    ```

#### Finding a Book

1. Select `Find Book` from the menu.
2. Enter the book title or author when prompted.

    ```plaintext
    ? What would you like to do? (Use arrow keys)
      Add Book 
    ❯ Find Book 
      List Books 
      Exit 
    ? Enter the book title or author to search: Gatsby
    ```

    Output:

    ```plaintext
    Books found:
    The Great Gatsby by F. Scott Fitzgerald
    ```

3. You can also search by a partial title or author name. For example, entering "Fitz" will match "F. Scott Fitzgerald".

    ```plaintext
    ? What would you like to do? (Use arrow keys)
      Add Book 
    ❯ Find Book 
      List Books 
      Exit 
    ? Enter the book title or author to search: Fitz
    ```

    Output:

    ```plaintext
    Books found:
    The Great Gatsby by F. Scott Fitzgerald
    ```

#### Listing Books

1. Select `List Books` from the menu.

    ```plaintext
    ? What would you like to do? (Use arrow keys)
      Add Book 
      Find Book 
    ❯ List Books 
      Exit 
    ```

    Output:

    ```plaintext
    Available Books:
    The Great Gatsby by F. Scott Fitzgerald
    ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
