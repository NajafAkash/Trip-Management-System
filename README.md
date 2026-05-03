# Trip-Management-System
The Trip Management System is a standard Desktop Application for educational institutions to plan, manage, and track student trips. It handles the full lifecycle from trip creation to reporting.

## 🚀 How the Application Works

1.Launch: Run the application to open the Authentication (Login/Registration) window.

2.Registration: New users register with an email and password. The system handles different roles: Student, Teacher, and Staff.

3.Login: Users log in to access their specific dashboard based on their role.

4.Student/Teacher Interaction:
Browse available trips in a list view.
Submit a "Trip Application" intent for a         specific destination.
The application sits in a "Pending" state, effectively decrementing the seat count temporarily.

5. Admin/Staff Interaction:
Staff members manage the master trip list (Add/Delete/Update).
Admins review the "Pending Requests" queue.
Approving a request finalizes the booking; declining it restores the seat count to the trip.
Staf/ Teacher can activate/Deactivate/Delete user accounts.

6.Persistence: All data is saved to local `.txt` files using Java Serialization, ensuring information is kept after closing the app.

✨ Key Features

** Role-Based Access Control**: Separate interfaces and permissions for Students, Teachers, and Staff members.

** Trip Approval Workflow: A robust request-queue system (Command Pattern) that allows manual verification before finalizing bookings.

** Dynamic Seat Management:Automatic tracking of available seats that updates in real-time as requests are processed.

** Persistent Data Storage: Uses a static database structure (Singleton-like) and file serialization to keep user and trip data persistent.

** Professional GUI: Built using Java Swing with organized layouts (GridBagLayout) for a clean user experience.

** Input Validation: Built-in error handling with user-friendly messages for invalid inputs or duplicate registrations.

🛠️ Design Patterns Used

** Singleton Pattern: Ensures data consistency across all application windows.

** Command Pattern: Manages the asynchronous Pending Request" and "Approval" system.

** Model-View-Controller (MVC): Separates the data logic from the graphical interface for better maintainability.
