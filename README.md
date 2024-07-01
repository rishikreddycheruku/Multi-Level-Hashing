# Multi-Level-Hashing
Representation of Multilevel Hash Table using User Interface Design

This project demonstrates a multilevel hash table implemented using HTML, CSS, and JavaScript. The hash table uses a two-level structure to handle hash collisions efficiently. This README provides an overview of the project, how to set it up, and how to use it.

## Project Structure

The project consists of a single HTML file that includes embedded CSS and JavaScript. The HTML file contains the structure of the webpage, the CSS styles define the appearance, and the JavaScript handles the functionality of the multilevel hash table.

## Features

Input Form: Users can input a value and the size of the hash table.
First Level Hash Table: Displays the main array after hashing the input values.
Second Level Hash Table: Displays sub-arrays to handle collisions using a secondary hash function.
Responsive Design: The layout adjusts based on the size of the input array.

## How It Works

1. Input Handling: Users enter a value and the size of the hash table. The `addValue` function processes the input and calculates the appropriate index using the hash function.
2. Hash Function: The primary index is calculated using `value % size`. If a collision occurs, the secondary index is calculated using `value % (size + 1)`.
3. Collision Handling: If a collision occurs (i.e., the primary index is already occupied), the value is stored in a secondary hash table (sub-array).
4. Display: The `displayArray` function updates the HTML to display the current state of the hash table, including both the main array and any sub-arrays.

## Usage

1. Open the HTML file in a web browser.
2. Enter a value in the "Value" input field.
3. Enter the desired size of the hash table in the "Array Size" input field.
4. Click the "Add Value" button to add the value to the hash table.
5. The main array and sub-arrays will be displayed, showing the current state of the hash table.

## Code Overview

### HTML Structure

Container: Holds the entire content and centers it.
Input Container: Contains input fields and the "Add Value" button.
Main Array: Displays the primary hash table.
Sub-array Container: Displays the secondary hash tables.

### CSS Styling

Main Array Boxes: Styled with a background color of orange and white text.
Sub-array Boxes: Styled with a background color of sky blue and white text.
Input Fields and Button: Styled for a consistent and appealing look.

### JavaScript Functionality

addValue Function: Handles the logic for adding values to the hash table.
displayArray Function: Updates the HTML to reflect the current state of the hash table.

## Example
1. Set the array size to 5.
2. Add the value 10. It will be placed at index 10 % 5 = 0 in the main array.
3. Add the value 15. It will also be placed at index 15 % 5 = 0, causing a collision. The value will be moved to a sub-array.
4. Continue adding values and observe how the hash table handles collisions and updates the visual representation.
