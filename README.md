# Invoice Management System

This is a C program for managing invoices. It allows users to create, read, update, and delete invoices. Invoice data is stored in a binary file `factura.dat`.

## Features

1. **Create Invoice**: Allows you to enter the details of a new invoice, including the client's name, ID, purchased products, quantities, and prices.
2. **Read Invoices**: Displays all stored invoices, excluding those marked as deleted.
3. **Search Invoice by ID**: Allows you to search for a specific invoice by the client's ID.
4. **Update Invoice**: Allows you to modify the details of an existing invoice, including the client's name, ID, products, and quantities.
5. **Delete Invoice**: Marks an invoice as deleted without physically removing it from the file.

## Code Structure

The code is organized into several functions, each responsible for a specific operation on the invoices:

### `menu()`
Displays the menu options for interacting with the system.

### `save()`
Saves a new invoice to the `factura.dat` file.

### `leercadena()`
Reads a string of text with a specific number of characters, cleaning the input buffer.

### `createFactura()`
Allows creating a new invoice, entering customer and product details, and saving the invoice.

### `readFactura()`
Reads and displays all invoices stored in the file.

### `findfacturabycedula()`
Searches for an invoice by the client's ID and displays its details.

### `updatefactura()`
Allows updating the details of an existing invoice.

### `deletefactura()`
Marks an invoice as deleted without physically removing it from the file.

## Requirements

- C Compiler (e.g., GCC)
- Operating system compatible with C (Windows, Linux, macOS)

## How to Use

1. Compile the source code:
    ```bash
    gcc -o invoice_management invoice_management.c
    ```

2. Run the program:
    ```bash
    ./invoice_management
    ```

3. Interact with the system using the menu options.

## Notes

- Deleted invoices are not physically removed from the file, they are marked with a special state.
- The `factura.dat` file is managed in a binary format.
