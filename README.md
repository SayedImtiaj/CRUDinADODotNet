# CRUDinADODotNet

## Overview

**CRUDinADODotNet** is a Windows Forms application developed in C# that provides functionality for managing student records using ADO.NET. The application supports creating, reading, updating, and deleting student information, including handling images. It also includes a login mechanism for accessing the application.

## Features

- **Student Management**: Add, update, delete, and view student records.
- **Image Handling**: Upload and display student images.
- **Login System**: Secure login to access the application.
- **Data Storage**: Stores data in a SQL Server database.

## Database Setup

### Database Creation

1. **Database**: `StudentInfoDB`
2. **Table**: `Student`
   - **StudentId**: Unique identifier, auto-incremented.
   - **Name**: Student's name.
   - **DOB**: Date of birth.
   - **Gender**: Gender of the student.
   - **Picture**: Path to the student's picture.

### Modifications

- **Added Columns**: `Picture` column to store image paths.
- **Extended `DOB` Column**: Updated the length of `DOB` to accommodate larger values.

## Application Components

### Forms

1. **Login Form**
   - **Purpose**: Authenticate users before accessing the application.
   - **Features**: User login validation against the `Users` table.

2. **Main Form (Form1)**
   - **Purpose**: Manage student records.
   - **Features**:
     - **Add**: Insert new student records into the database.
     - **Update**: Modify existing student records.
     - **Delete**: Remove student records.
     - **View**: Display student records in a DataGridView.
     - **Image Handling**: Upload and display student images.

### Reports

- **Crystal Reports Integration**: Allows for generating and viewing reports of student data.

## Setup Instructions

### Prerequisites

- **Visual Studio 2019** or later
- **SQL Server** (LocalDB is recommended for development)
- **Crystal Reports** for Visual Studio

### Installation Steps

1. **Clone the Repository**

   Clone the project repository to your local machine.

2. **Open in Visual Studio**

   Open the solution file (`CRUDinADODotNet.sln`) in Visual Studio.

3. **Database Configuration**

   Ensure the SQL Server database (`StudentInfoDB`) is attached. Adjust the connection string in `App.config` if needed to match your SQL Server setup.

4. **Build and Run**

   Build the solution in Visual Studio and run the application to manage student records.

## Usage

- **Login**: Use the login form to access the main application.
- **Manage Students**: Use the main form to add, update, delete, and view student records.
- **Upload Images**: Upload student images and view them in the application.
- **Reports**: Generate and view reports on student data using Crystal Reports.

## Contribution

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. For more details, see the [LICENSE](LICENSE) file.

## Contact

For questions, suggestions, or issues, please contact the project maintainer at [your.email@example.com](mailto:your.email@example.com).

---

Feel free to modify any sections or add additional details as needed!
