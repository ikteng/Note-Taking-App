# Note-Taking-App

This Python code defines a simple note-taking application using PyQt6 for the GUI and SQLite for database storage.

## GUI Layout
- The application window consists of a main layout divided into 2 sections: a sidebar on the left and a note input area on the right. These sections are managed using a QSplitter to allow resizing.
- The sidebar contains a list of notes and a button to create a new note.
- The note input area contains fields for entering the name and content of a note.

## Menu Bar
- The application has a menu bar with three menus: File, Edit, and View.
- The File menu contains options for creating new notes, opening existing notes, saving notes, and exiting the application.
- The Edit menu contains options for undoing and redoing actions.
- The View menu contains options for showing or hiding the sidebar.

## Sidebar
- The sidebar is implemented using a QListWidget and contains a list of notes.
- Users can create new notes, edit existing notes, and delete notes from the sidebar.
- The sidebar also supports copy, paste, and cut functionalities for notes.
- Each note in the sidebar is represented by an item in the list.

## Note Input Area
- Below the sidebar, there's an area for inputting note names and contents.
- It consists of QLineEdit for entering note names and QTextEdit for entering note contents.
- Users can add new notes, edit existing notes, and delete notes using this input area.

## Clipboard
The application maintains a clipboard for storing copied or cut notes.

## Data Persistence
- Notes are stored in a SQLite database named "notes.db" to ensure data persistence across sessions.
- When the application starts, it loads existing notes from the database into the sidebar.
- Notes are saved to the database when the application is closed.

## Error Handling
Error handling is implemented for file operations and database interactions, displaying error messages when necessary.

## File Import and Export
- Users can import notes from text files and export notes as text files.
- Importing a text file adds its content as a new note, while exporting a note saves its content to a text file.

## View Management
Users can show or hide the sidebar using options in the View menu.
