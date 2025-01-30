# AbstractClassesUML


###### Project Overview
This project focuses on designing and implementing abstract classes for a console-based application while visualizing the class structure using UML diagrams. The goal is to create an extendable and modular architecture where user interfaces can be easily modified or extended.

## Objectives
- Design UML class diagrams to represent the structure of an application.
- Implement an abstract base class for user interfaces.
- Create a concrete implementation of a console-based user interface.
- Modify the existing application to support flexible UI representations.

## UML Diagram
The UML class diagram below represents the structure of the application and its relationships between components:

- **UserInterface (Abstract Class)**
  - `display_menu()`
  - `display_contacts(contacts)`
  - `display_notes(notes)`
  - `display_commands()`
  
- **ConsoleUserInterface (Concrete Class)**
  - Implements all methods from `UserInterface`
  
- **Menu (Class)**
  - `choices` (Dictionary of available modules)
  - `user_interface` (Instance of `UserInterface`)
  - `make_decision(choice)` (Handles user input and executes corresponding module)

- **Module Functions**
  - `calend_main()` (Calendar module)
  - `start_ab()` (Address Book module)
  - `notebook()` (Notebook module)
  - `start_fs()` (File Sorter module)
  - `ex_main()` (Exchange Rate module)

## Installation & Usage
### Prerequisites
- Python 3.x

### Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/paulmusquaro/AbstractClassesUML.git
   ```
2. Navigate to the project directory:
   ```sh
   cd AbstractClassesUML
   ```
3. Run the application:
   ```sh
   python menu.py
   ```

### How to Use
- Run `menu.py` and follow the on-screen instructions.
- Choose a module from the menu to interact with different functionalities.
- Modify `ConsoleUserInterface` or create new UI implementations for different outputs (e.g., GUI, Web-based UI).

## License
This project is open-source and available under the MIT License.