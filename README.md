# Termsheet-Validator-AI

## Overview:

The TermSheet AI Validator is a web-based interface designed to assist Middle Office staff (e.g. analysts like Sagar) in processing, validating and managing term sheets. Built with HTML, CSS and JavaScript, this provides a hub to upload documents, review results and correct the errors. It integrates AI-driven validation capabilities and is intended to connect with backend systems for full functionality.(I will need some time)

The current version is a front-end prototype demonstrating the layout and basic interactivity of the and Detailed View (Manual Corrections) screens.


# Login Page

The login page, is essential for secure access(not coded but hypothetical). It mainly includes an email input field, password field (with visibility toggle icon, e.g., eye symbol), and a blue "Sign In" button. Below, a "Forgot Password?" link leads to recovery, with a footer for copyright and terms (e.g. "© 2025, Terms of Use"). This design is a normal Login Page examples which ensures a user-friendly and secure entry for Middle Office staff.


# Main Page

## Dashboard
The main page, is the dashboard hub, crucial for Middle Office staff. It features a header with the title "TermSheet AI Validator", user info (e.g. "Sagar | Analyst,"), and date. A fixed sidebar offers navigation (Dashboard, Upload Documents, etc.) with icons, active in blue and hover effects (grey). 

The main content includes a full-width search bar with a magnifying glass icon, filter buttons and three summary cards: 
- Processed Today (blue, "50," subtext "245 this week") 
- Errors Flagged (red, "5," subtext "3 pending") 
- Processing Time (green, "2 min/sheet," subtext "1.5 min fastest"). 
- Notifications list alerts with a "Dismiss All" button. 
- A chart placeholder showing error rate trends(e.g. bar chart).


## Upload Documents Webpage 
The Upload Documents webpage allows file uploads with a drag-and-drop area (300x150px) and an "Upload File" button. Users select document type (PDF, Word, HTML, Excel) via a dropdown and optionally enter a batch ID. A progress bar simulates uploads, showing "Uploading: 60%." The layout is clean and centered, ensuring ease of use for Middle Office staff.


## Error Logs Webpage 
The Error Logs webpage lists errors in a table, color-coded along with trade ID, error type, description, counterparty, timestamp and a "View" button. A red warning banner shows unresolved errors (e.g. "2"), clickable for filtering, aiding quick error resolution.


## Manual Corrections Webpage 
The Manual Corrections webpage displays a split panel: left shows editable fields (Trade ID, Company Name,..) with pencil icons for edits; right shows validation status (e.g. "Flagged" in red) and checks (pass/fail). Action buttons (Correct & Resubmit, yellow; Approve Anyway, orange; Reject, red) allow decisions, with notes and escalation options. A history log tracks actions (e.g. "Edited Payment at 10:20 AM").





# Usage

1) Navigate the Dashboard:
- Click sidebar items (e.g., "Upload Documents") to switch sections.
- Use the "Back to Dashboard" button in Manual Corrections to return to the main view.


2) Upload Documents:
- Click "Upload File" to select a file (displays filename).
- Choose a document type and optionally enter a batch ID.
- Click "Submit" to simulate an upload with a progress bar.


3) Review and Edit Term Sheets:
- In "Error Logs," click "View" to open Manual Corrections for a specific term sheet.
- Edit fields (e.g., Payment Terms) by clicking the pencil icon, then save or cancel changes.


4) Analytics:
- Toggle between Flow Chart and Pie Chart placeholders to preview diagram types.



## Technologies Used

1) Core Development & Logic
- HTML: Structures the dashboard layout and content.
- CSS: Styles the interface with inline rules for layout, colors, and spacing.
- JavaScript: Adds basic interactivity (section toggling, field editing, file upload simulation).


2) Planned Backend Integration (In process, Not Included)
- Python (Flask)
- APIs


3) Planned AI & Data Processing (In process, Not Included)
- Tesseract
- spaCy
- Scikit-learn
