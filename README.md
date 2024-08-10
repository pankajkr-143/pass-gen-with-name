# pass-gen-with-name
Here's a detailed note for your GitHub README file:

---

# Password Generator and Storage Application

This application is a simple Python-based tool that automatically generates a secure password based on a given name and desired password length. The application stores the generated name and password pairs in a SQLite3 database, providing an easy way to manage and secure your passwords.

## Features

- **Password Generation**: Automatically generates a strong password based on user-defined length.
- **Data Storage**: Stores the name and corresponding generated password in a SQLite3 database.
- **Add Data**: Allows users to input a name and password length to generate and store a password.
- **Reset Data**: Provides an option to clear all stored data from the database.

## How It Works

1. **Input**: The user provides a name and the desired length of the password.
2. **Password Generation**: The application uses Python's `random` library to generate a secure password containing a mix of uppercase letters, lowercase letters, numbers, and special characters.
3. **Data Storage**: The generated name and password pair is stored in a SQLite3 database.
4. **Reset Data**: Users can clear all the stored name and password pairs from the database by choosing the reset option.

## Technologies Used

- **Python**: The core programming language used for the application logic.
- **SQLite3**: A lightweight, disk-based database used to store name and password pairs.

## Prerequisites

Before running the application, ensure you have Python installed on your machine. SQLite3 is included with Python by default.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/pankajkr-143/pass-gen-with-name.git
   ```
2. Navigate to the project directory:
   ```bash
   cd pass-gen-with-name
   ```

## Usage

1. **Run the Application**:
   ```bash
   python main.py
   ```
   
2. **Add Data**:
   - Input a name.
   - Enter the desired length for the password.
   - The application will generate a secure password and store it in the database when you click on Accept.

3. **Reset Data**:
   - Choose the reset option to clear all stored data.

## Code Overview

### Main Python Script (`main.py`)

- **Password Generation Function**: 
  - Generates a password with a specified length using a mix of characters.
  
- **Database Interaction**:
  - Connects to an SQLite3 database.
  - Creates a table if it does not exist.
  - Inserts the name and generated password into the database.
  - Deletes all records from the database when the reset option is selected.

### SQLite3 Database (`users.db`)

- The database consists of a single table named `passwords`, which stores the following:
  - **ID**: An auto-incremented primary key.
  - **Name**: The name associated with the password.
  - **Password**: The generated password.

## Example

1. **Generate a Password**:
   - Input: Name = "example", Password Length = 12
   - Output: Password = "A8d#kLm7B2!p"

2. **Database Record**:
   - Name: "example"
   - Password: "A8d#kLm7B2!p"

## Contributing

Feel free to fork this repository and make contributions. Pull requests are welcome!

## License

This project is licensed under the Macky's Tech License. See the LICENSE file for details.

---

This note should give users a clear understanding of what the application does, how to use it, and how it works.

**How it work you can watch**

https://github.com/user-attachments/assets/fa32aac8-6a9c-4318-84c8-e269b6342cef



