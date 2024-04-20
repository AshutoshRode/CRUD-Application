# User Management System

This project is an Angular-based User Management System designed to demonstrate basic CRUD (Create, Read, Update, Delete) operations in a simple user interface. The application is divided into various modules, specifically focusing on user operations. It includes a reactive form for user data entry, validation, and a grid display of users with options to edit or delete records.

## Features

- **User Module**: Manages all user-related functionalities.
- **Reactive Forms**: Utilizes Angular's reactive forms for capturing user data.
- **CRUD Operations**: Supports adding, updating, and deleting users.
- **Validation**: Ensures that user data is validated before submission.
- **Data Passing**: Uses a DataService for inter-component communication.
- **Responsive UI**: Styled using Bootstrap to ensure the application is visually appealing and responsive.

## Project Setup

1. **Clone the repository:**

```bash
git clone https://github.com/AshutoshRode/User-Management-System.git
cd User-Management-System
```

2. **Install dependencies:**

```bash
npm install
```

3. **Run the development server:**

```bash
ng serve
```

Open [http://localhost:4200/](http://localhost:4200/) to view it in the browser.

## Project Structure

- `src/app/user/` - Contains all the components and services related to user management.
  - `user.module.ts` - The module file for user features.
    - `user-upsert/` - Component for creating and updating user details.
    - `user-list/` - Component for displaying the list of users.
- `src/app/shared/` - Contains shared utilities, models, and services.
  - `data.service.ts` - Service for managing and passing data between components.
- `db.json`- for json server dummy API

## Components

### User-Upsert Component

- **Form Fields**: FirstName, LastName, Address, Email, Phone.
- **Validations**: Required fields, email format, and phone number length.
- **Operations**: Handles both adding new users and updating existing ones based on the presence of a unique ID.

### User-List Component

- **Display**: Shows all users in a responsive grid with options to edit or delete.
- **Actions**: Each row has buttons for editing and deleting users, interfacing directly with the User-Upsert Component for seamless data flow.

## Services

### DataService

- **Purpose**: Manages the transfer of data between the User-List and User-Upsert components and controls the refresh of the user list on data update.

## Styling

- **Framework**: Bootstrap is integrated for responsive design and quick styling capabilities.
- **Custom Styles**: Additional styles can be added in the respective component's CSS files.

## Additional Features


- **Dummy Data**: Initially populates user data from a JSON server dummy API to simulate a real environment.






step 1:-> 
   download repository zip file

step 2:->
   extract zip file

step 3:->
   open terminal in "user-management-system" file      

step 4:->
   run 
      npm install

step 5:->
    run 
       ng serve

step 6:->
    open new terminal ,install json server
    run 
       npm install json-server
       
step 7:->
    run
       json-server --watch db.json
        


