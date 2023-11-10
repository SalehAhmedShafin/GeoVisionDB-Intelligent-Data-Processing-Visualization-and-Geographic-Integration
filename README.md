# Test-for-Middle-Python-Developer-Machine-Learning-AI
This repository contains-
- [Creating a neural network](#Introductions)
- [Working with databases](#Troubleshooting)
- [Integration with a Google API](#Overview)


# Deep Neural Network for MNIST
A deep neural network implemented in PyTorch for recognizing handwritten digits from the MNIST dataset.

## Table of Contents

- [Introduction](#introductions)
- [Installation](#installation)
- [Usage](#prerequisites)
- [Network Architecture](#network-architecture)
- [Hyperparameters](#hyperparameters)
- [Training](#training)
- [Testing](#testing)
- [Results](#results)
- [Troubleshooting](#troubleshooting)

## Introductions

This repository contains the source code for a deep neural network designed to classify handwritten digits using the MNIST dataset. The code is built with PyTorch and provides functionalities for training, testing, and evaluating the model.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/SalehAhmedShafin/Test-for-Middle-Python-Developer-Machine-Learning-AI
    cd https://github.com/SalehAhmedShafin/Test-for-Middle-Python-Developer-Machine-Learning-AI
    ```

2. Install dependencies:

    ```bash
    pip install torch torchvision numpy matplotlib scikit-learn
    ```
### Prerequisites

- Python 3.x
- PyTorch (install via `pip install torch`)
- torchvision (install via `pip install torchvision`)
- Other dependencies: NumPy, Matplotlib, Scikit-learn (install via `pip install numpy matplotlib scikit-learn`)


### Network Architecture
The neural network architecture is defined in the DeepNeuralNetworkModel class. It consists of three hidden layers with ReLU activation functions and an output layer.

### Hyperparameters
Customize hyperparameters according to the requirements. Important hyperparameters include num_hidden, learning_rate, num_epochs, and batch_size.

### Training
The training process involves iterating over the training dataset, computing the loss, and updating the model parameters using gradient descent. The training loop is implemented in this file.

### Testing
Testing the model involves evaluating its performance on a separate test dataset. The testing code is implemented in this same file.

### Results
After training and testing, i can analyze the results, including accuracy, precision, recall, and F1-score, to assess the model's performance.

### Troubleshooting
If encounter any issues, please check the following:

- Ensure all dependencies are installed.
- Verify that the datasets are correctly loaded and preprocessed.
- Check for typos or errors in the configuration files.

# User Database Interaction

- [Introduction](#introduction)
- [Installation](#installation)
- [Database Structure](#database-structure)
- [Code Capabilities](#code-capabilities)
- [Usage](#usage)
- [Examples](#examples)

## Introduction

This repository contains Python code for interacting with a user database using SQLite. The code includes functions for inserting, updating, deleting, and retrieving user data.

## Installation

### Prerequisites

- Python installed on your system.
- SQLite database library (`sqlite3`) included with Python.

### Setup

1. Clone or download the repository.
2. Ensure that the required Python packages are installed:

    ```bash
    pip install sqlite3
    ```

3. Open the Python script or Jupyter notebook containing the code in your preferred editor.

## Database Structure

The database consists of a single table named `users` with the following structure:

- `id` (Primary Key): Unique identifier for each user.
- `username`: User's username.
- `email`: User's email address.

## Code Capabilities

### Functions

1. **`email_check(email)`**
   - Validates an email address using a regular expression.

2. **`insert_user(username, email)`**
   - Inserts a new user into the `users` table, ensuring data validity.

3. **`update_user(user_id, new_email)`**
   - Updates the email of a user with a specific `user_id`.

4. **`delete_user(user_id)`**
   - Deletes a user with a specific `user_id` from the `users` table.

5. **`all_users()`**
   - Retrieves and prints information about all users in the `users` table.

6. **`show_user(user_id)`**
   - Retrieves and returns information about a specific user with the given `user_id`.

## Usage

1. **Import the Code:**
   - Import the functions into your Python script or Jupyter notebook:

    ```python
    import sqlite3
    ```

2. **Establish Database Connection:**
   - Create a connection and cursor:

    ```python
    conn = sqlite3.connect('User_Database.db')
    cursor = conn.cursor()
    ```

3. **Use the Functions:**
   - Utilize the functions for various user database interactions.

4. **Commit Changes and Close Connection:**
   - Always commit changes and close the connection when done:

    ```python
    conn.commit()
    cursor.close()
    conn.close()
    ```

## Examples

```python
# Insert Users
insert_user('Saleh', 'saleh@gmail.com')
insert_user('Shafin', 'shafin@gmail.com')

# Display All Users
print("All Users:")
all_users()

# Update User Email
update_user(1, 'ahmedsaleh@gmail.com')

# Show User Information
print("User ID 1 is: ", show_user(1))

# Delete User
delete_user(2)
print("User with ID 2 deleted Successfully.")

# Display All Users Again
print("All Users After Deletion:")
all_users()
 ```




# Google Maps API Integration with Selenium and Python

## Overview

This Python script demonstrates the integration of the Google Maps JavaScript API using Selenium. It generates a simple HTML file containing a Google Map and opens it in a web browser for visualization.

## Features

- **Google Maps Integration:** Embeds a Google Map in an HTML file using the Google Maps JavaScript API.
- **Dynamic API Key:** Allows users to replace the placeholder API key with their own Google Maps API key.
- **Selenium Automation:** Utilizes Selenium to open the generated HTML file in a web browser.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Configuration](#configuration)
- [Error Handling](#error-handling)
- [Logging](#logging)
- [Troubleshooting](#troubleshooting)
- [Acknowledgments](#acknowledgments)

## Installation

### Prerequisites

- Python installed ([Download Python](https://www.python.org/))
- Chrome WebDriver installed ([Download Chrome WebDriver](https://sites.google.com/chromium.org/driver/))

### Install Dependencies

```bash
pip install selenium
```

## Usage
1. Replace API Key:
   - Replace the placeholder API key ('YOUR_API_KEY') in the script with your valid Google Maps API key.
2. Run the Script:
   - Ensure that the Chrome WebDriver is in system's PATH.
   - The script will generate an HTML file (google_maps.html) and open it in a Chrome browser.
    
## Customization
1. Adjust Map Settings:
   - Modify the initMap function in the script to customize the initial center and zoom level of the map.
      
## Configuration
1. API Key Configuration:
    - Store API keys and other configuration parameters in a configuration file for better management.

## Error Handling
1. Exception Handling:
    - The script includes basic exception handling. Ensure to handle exceptions appropriately in a production environment.

## Logging
1. Logging:
    - The script includes basic logging for informational purposes. Adjust the logging configuration based on your needs.

## Troubleshooting
1. WebDriver Issues:
    - If the script fails due to WebDriver issues, ensure the correct path to the Chrome WebDriver is specified.
API Key Errors:

If the map doesn't load, check the browser console for any errors related to the Google Maps API key.


## Acknowledgments
- The script uses Selenium for browser automation (Selenium).
- Google Maps API documentation: Google Maps JavaScript API Documentation
