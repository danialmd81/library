# Library Management System

A comprehensive library management system built with C++ that implements advanced data structures including AVL Trees, Linked Lists, and Queues. This project demonstrates the application of data structure concepts in a real-world scenario.

## Project Overview

This Library Management System allows for efficient management of books, users, and administrative tasks within a library environment. It features a command-line interface with color-coded interactions and intuitive navigation options.

### Authors

- Danial Mobini (40130023)  
- Mohammad Sadegh Hatefi (40133073)
- Hadis Kianpour (40201763)

## Features

### User Management

- User registration and authentication
- Book borrowing and returning
- Book reservation system
- Viewing personal book list
- Requesting time extensions for borrowed books
- Penalty system for late returns

### Admin Management

- Admin authentication (default credentials: username: `admin`, password: `1234`)
- Book management (add, assign, retrieve)
- User management (add, view details)
- Extending book reservation times
- Complete book inventory management

### Book System

- Book categorization with title, genre, publication date, and author
- Book assignment and reservation tracking
- Time-based handling for book loans and reservations
- Queue-based reservation system

## Data Structures Implemented

This project showcases several advanced data structures:

1. **AVL Tree**: Self-balancing binary search tree used for efficient book searching and sorting
2. **Linked List**: Used for managing collections of books and users
3. **Queue**: Implements the reservation system for books

## System Policies

The system enforces several library policies:

- Book borrowing period: 10 days
- Reservation claim deadline: 3 days
- Late return penalty: 5 units per day after the deadline

## Technical Details

### Dependencies

- C++ (C++23 standard)
- Boost library (for date/time handling)
- Cereal library (for JSON serialization)

### Data Persistence

The system uses JSON file storage (`library.json`) to maintain data between sessions, ensuring all information about books, users, and reservations is preserved.

### Compilation

The project can be compiled using G++ with the C++23 standard:

```bash
g++ -Wall -std=c++23 *.cpp -o library.exe -I <path_to_include_directory>
```

## Usage

1. Run the executable
2. Choose between Admin and User interfaces
3. For admin access, use the default credentials (username: `admin`, password: `1234`)
4. For user access, either register a new account or log in with existing credentials

### Admin Operations

- Adding new books to the library
- Adding new users to the system
- Assigning books to users
- Retrieving books from users
- Extending reservation times
- Viewing detailed user information

### User Operations

- Borrowing available books
- Returning borrowed books
- Requesting time extensions for borrowed books
- Viewing personal book collection
- Browsing the full library catalog
- Searching for specific books

## Implementation Highlights

- Color-coded terminal interface for better user experience
- Progress bar animations for system operations
- Self-balancing AVL tree for efficient book searching
- Time-tracking mechanism for loan periods and reservations
- Queue-based reservation system for fair book allocation
- JSON serialization for persistent data storage
