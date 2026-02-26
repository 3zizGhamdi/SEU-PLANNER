# SEU Planner

A lightweight, offline-friendly planner for SEU courses that helps you manage weekly lecture times and track due dates for exams, discussions, assignments, projects, and quizzes.

## Features
- Separate tables for each activity type (Lectures, Exams, Discussions, Assignments, Projects, Quizzes)
- Live “Time left” countdown for deadlines
- Mark items as Done / Undo
- Add / Edit / Delete entries at any time
- English/Arabic toggle with RTL/LTR support
- Optional browser notifications (24h and 12h reminders)

## How it works
- Your data is stored locally in your browser using the Web Storage API (`localStorage`), so it persists after closing and reopening the browser on the same device. [web:16][web:17]
- Notifications use the Web Notifications API and require user permission (`Notification.requestPermission()`). [web:35]

## Getting started
1. Download the project or clone the repository.
2. Open `index.html` in your browser (no server required).

## Usage
- To add an item: fill the fields in the top row of a table and click **Add**.
- To edit an item: click **Edit** and update the prompted fields.
- To delete an item: click **Delete**.
- To reset everything: click **Clear all** (this removes saved data from this device).

## Default data (Auto-filled)
This version includes a one-time “seed” that preloads the provided courses and dates on the first run. After that, you can freely modify or remove them, and the app will keep your changes in `localStorage`. [web:16]

## Notes
- `datetime-local` values use the format `YYYY-MM-DDTHH:mm` (example: `2026-04-02T19:00`).  
- If notifications are blocked, enable them in your browser/site settings and try again. [web:35]

## Author
Abdulaziz Alghamdi
