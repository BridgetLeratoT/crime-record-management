#Crime Record Management System



The Crime Record Management System is a secure and systematic way of maintaining criminal and case records. Admin users can input and update crime cases, suspect profiles, evidence details, and investigation reports. Search and filtering functionalities allow quick access to data based on date, location, or type of crime. 

This project helps law enforcement or legal students understand the data flow in criminal justice systems. It is a robust example of secure CRUD operations, data management, and modular application design in Java.
steps to create crime record management

    Define entities — cases, suspects, evidence.

    Design data entry forms.

    Create Case, Suspect classes.

    Implement search and update functions.

    Store data securely in DB.

    Add report generation.

    Test data CRUD and searches.

    Add authentication for security.

    Document system.

    Package for use.

code explanation

1.  CrimeRecord Class
 

class CrimeRecord {
    String id, crimeType, location, accusedName, officer;
}

    Holds the details of a single crime.

    Each record has:

        Crime ID

        Crime Type

        Location

        Accused Name

        Officer In Charge

2.  CrimeRecordSystem GUI

Main class that extends JFrame to create a Swing-based GUI.
 Left Panel – Add Crime Record

    Fields:

        Crime ID

        Crime Type (dropdown)

        Location

        Accused Name

        Officer In Charge

    Buttons:

        "Add Record" – Adds the crime record to the list

        "Search Crime Type" – Filters by crime type

 Center – Table to Display Records
JTable table;

    Shows a list of all crime records

    Columns: ID, Crime Type, Location, Accused, Officer

 Bottom – Search & Delete

    Search field to search crime type

    Show All – Displays all records

    Delete Selected – Deletes the selected row from the table

