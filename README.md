# Inverted Search (C)

## Overview
Inverted Search is a C-based application that builds an inverted index for efficient text searching across multiple files. Instead of searching files line by line, the program maps each unique word to the list of files in which it appears along with its frequency.

This project demonstrates the practical use of data structures, file handling, and algorithmic thinking, making it suitable for system programming and embedded software roles.

## Features
- Create an inverted index from multiple text files
- Search for a word across all indexed files
- Display file names and word occurrence counts
- Efficient searching using linked lists
- Menu-driven console application
- Supports dynamic number of input files

## Technologies Used
- Language: C
- Concepts:
  - Linked lists
  - File handling
  - String manipulation
  - Dynamic memory allocation
  - Modular programming
  - Searching algorithms

## Project Flow

### Index Creation
1. Read file names from command-line arguments.
2. Open each file and read words one by one.
3. Store each unique word in the main linked list.
4. For every word, maintain a sub-linked list of file names and word counts.
5. Build the complete inverted index in memory.

### Searching
1. Accept a search word from the user.
2. Traverse the inverted index.
3. If the word is found, display all files containing the word and its frequency.
4. If not found, display an appropriate message.

## Usage

### Compilation
gcc *.c -o inverted_search

### Execution
./inverted_search file1.txt file2.txt file3.txt

### Sample Operations
- Create database
- Display database
- Search a word
- Exit

## Project Structure
Inverted-Search/
│
├── create_db.c
├── search_db.c
├── display_db.c
├── file_validation.c
├── types.h
├── main.c
└── README.md

## Limitations
- Case-sensitive search (unless normalized)
- Supports text files only
- In-memory database (not persistent)

## Future Enhancements
- Add file persistence for database
- Implement case-insensitive search
- Optimize using hash tables
- Support large-scale datasets

## Learning Outcomes
- Strong understanding of inverted indexing
- Hands-on experience with linked lists
- Improved searching and data organization skills
- Practical exposure to real-world search engine concepts

## Author
Syed Shifan Ali
