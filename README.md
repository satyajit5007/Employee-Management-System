# Employee Management System (C++)

A console-based Employee Management System built in C++ that allows user registration, login, and complete CRUD (Create, Read, Update, Delete) operations for employee records.  
---

## Features

- **User Authentication**  
  - Registration and Login system with secure password input.
- **Employee Data Management**  
  - Add new employee records.
  - View all employee records.
  - Modify existing employee details.
  - Search for an employee by ID.
  - Delete employee records.
- **Persistent Storage**  
  - Data is stored in text files (`Employee_Record.txt` and `Ep_data.txt`).

---

## File Structure

```

.
├── Employee\_Management.cpp    # Main source code
├── Employee\_Record.txt        # Stores employee data
├── Ep\_data.txt                # Stores user credentials
└── README.md                  # Project documentation

````

---

## Requirements

- **Operating System:** Windows (uses `windows.h` and `conio.h`)
- **Compiler:** Any C++ compiler supporting C++11 or later
- **Libraries Used:**
  - `<iostream>`
  - `<fstream>`
  - `<cstring>`
  - `<cstdlib>`
  - `<conio.h>` (Windows only)
  - `<windows.h>` (Windows only)
  - `<unistd.h>` (POSIX sleep function, Windows alternative via `Sleep()`)

---

## How to Run

1. **Clone the repository or copy the source code**:
   ```bash
   git clone https://github.com/satyajit5007/employee-management-system.git
   cd employee-management-system
````

2. **Compile the program**:

   ```bash
   g++ Employee_Management.cpp -o employee.exe
   ```

3. **Run the program**:

   ```bash
   ./employee.exe
   ```

---

## Usage Guide

1. **Login or Register**

   * First-time users must register with a username and password.
   * Existing users can log in directly.

2. **Menu Options**

   ```
   1. Enter New Record
   2. Display Record
   3. Modify Record
   4. Search Record
   5. Delete Record
   6. Exit
   ```

3. **Data Storage**

   * Employee data is stored in `Employee_Record.txt`
   * Login credentials are stored in `Ep_data.txt`

---

## Example Data Format

**Employee\_Record.txt**

```
John 1001 Manager 35 75000 10yrs
Alice 1002 Developer 28 60000 4yrs
```

**Ep\_data.txt**

```
admin admin123
user1 pass1
```

---

## Limitations

* Windows-specific due to `windows.h` and `conio.h`.
* No encryption for stored passwords.
* No validation for duplicate Employee IDs.
* Basic text-based interface without GUI.

---

## Future Improvements

* Encrypt stored passwords.
* Add date of joining and contact details.
* Implement a cross-platform version (remove Windows-specific dependencies).
* Add sorting and filtering of employee records.

---