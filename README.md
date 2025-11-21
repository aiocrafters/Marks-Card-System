School Marks Card Generator

A web-based application to generate, view, and print student marks cards automatically. This system calculates totals and grades based on input data and formats it into a professional, print-ready A4 layout.

📂 Project Files

marks_card.html: The main application file containing the logic, user interface, and print layout.

students_db.json: The database file storing student details and marks.

🚀 How to Run the App

Because this application loads data from an external file (students_db.json) using the fetch API, browser security policies prevent it from running directly by double-clicking the HTML file. You must run it via a local server.

Option 1: Using VS Code (Recommended)

Install the Live Server extension in VS Code.

Open the folder containing marks_card.html and students_db.json in VS Code.

Right-click marks_card.html and select "Open with Live Server".

Option 2: Using Python

If you have Python installed, open your terminal/command prompt in the project folder and run:

# For Python 3
python -m http.server


Then open your browser and go to http://localhost:8000/marks_card.html.

🛠️ Features

Search Filters: Filter students by Class (9th/10th).

Smart Search: Search by Admission No, Roll No, or Name.

Dynamic Dropdown: The search input provides auto-suggestions based on the available data.

Auto-Calculation: Automatically computes FA Totals, Grand Totals, and Grades based on scores.

Print Ready: Clicking "Print" hides the search bar and formats the card perfectly for A4 paper.

📝 How to Add Students

Open students_db.json in any text editor and add a new object to the list following this format:

{
  "admNo": "104",
  "rollNo": "3",
  "class": "10th",
  "name": "New Student Name",
  "father": "Father Name",
  "mother": "Mother Name",
  "aadhaar": "XXXX-XXXX-XXXX",
  "dob": "YYYY-MM-DD",
  "contact": "9999999999",
  "category": "General",
  "gender": "Male/Female",
  "subjects": [
    { "name": "English", "fa1": 10, "fa2": 10, "fa3": 10, "sa1": 30, "sa2": 40 },
    // ... add other subjects
  ]
}


🖨️ Printing Tips

Use the Print button inside the app, not the browser's print option.

In the print preview window, ensure "Background graphics" is checked in the settings to see the table colors properly.

Set margins to "Default" or "None" for the best fit.