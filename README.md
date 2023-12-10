# Banking-Management
project for 533

## Overview
The AZYY Bank Management System is a Python package designed to simulate a simple banking system with user and admin functionalities. It includes features such as user registration, client and admin management, investment handling, and more.

# AZYY Bank Management System - Function Details

## Overview

The AZYY Bank Management System is built with several functions to manage user and admin interactions, as well as investment handling. Here, we provide details about key functions in the system.

## How to test?
Go to test.ipynb which is isolated from the requierd package "bank_management".
Then run this file.

```python
from bank_management import start
```
This block is used to import functional py file from the required package

```python
start.main()
```
Then this block is used to start our program.

## Continuous integration testing
We are using GitHub Action to help us test our package functions. The CI configuration file is stored in .github/workflow/

## Functions

### `clients_initialization()`

- **Description:** Initializes client objects with sample data.

- **Returns:** A dictionary containing client objects.

### `admins_initialization()`

- **Description:** Initializes admin objects with sample data.

- **Returns:** A dictionary containing admin objects.

### `investment_initialization()`

- **Description:** Initializes an empty dictionary for investment objects.

- **Returns:** An empty dictionary for investment objects.

### `mortgage_initialization()`, `zcb_initialization()`, `gov_initialization()`

- **Description:** Initializes dictionaries with sample data for different types of investments (mortgage, zero coupon bond, government bond).

- **Returns:** Dictionaries containing investment objects.

### `main()`

- **Description:** The main function that runs the AZYY Bank Management System. It prompts the user to choose a role (new user, existing client, admin, quit) and handles the corresponding actions.

### `personal_invest(c_new)`

- **Description:** Manages personal investments for a specific client.

- **Parameters:**
  - `c_new`: Client object.

### `test()`

- **Description:** A test function (currently commented out) that demonstrates the usage of the `admin_login()` function.


## Usage

To use the functions in this system, follow these steps:

1. **Initialize Clients, Admins, and Investments:**
   - Call `clients_initialization()` to initialize client data.
   - Call `admins_initialization()` to initialize admin data.
   - Call `investment_initialization()` to initialize an empty investment dictionary.
   - Call `mortgage_initialization()`, `zcb_initialization()`, and `gov_initialization()` to initialize investment dictionaries.

2. **Run the Main Function:**
   - Call `main()` to start the AZYY Bank Management System.
   - Choose your role (new user, existing client, admin, quit) and follow the on-screen instructions.

3. **Manage Personal Investments:**
   - If the user chooses the "Existing client" role, they can manage personal investments using the `personal_invest(c_new)` function.

4. **View All Investments:**
   - Call `show_all_investment(mortgage_dict, zcb_dict, gov_dict)` to display details of all available investments.

5. **Testing:**
   - Call `test()` to run a test function (currently commented out).

## Sample Data

Sample data for clients, admins, and investments is pre-initialized in the code.

## License

This project is licensed under the [MIT License](LICENSE).


