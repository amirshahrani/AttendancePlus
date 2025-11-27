# AttendancePlus

A JavaFX desktop application for tracking student attendance across university courses. Built as an Object-Oriented Programming project (Jan 2025).

## Features

- **User Authentication** - Login and sign-up functionality with local file-based storage
- **Interactive Calendar** - Navigate through months and select dates to view scheduled classes
- **Daily Schedule View** - Displays courses scheduled for the selected day with location and time
- **Attendance Tracking** - Mark attendance for current day classes with Present/Absent status
- **Attendance Statistics** - View attendance ratio per subject with color-coded indicators (green ≥90%, red <90%)
- **Reminders Panel** - Dedicated window for managing reminders

## Screenshots

| ![Dashboard](./src/main/resources/com/attendance/plus/attendanceplus/images/screenshots/Dashboard-1.png) | ![Dashboard Stats](./src/main/resources/com/attendance/plus/attendanceplus/images/screenshots/Dashboard-2.png) |
| :------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------: |
|                                         Dashboard with Calendar                                          |                                             Attendance Statistics                                              |

| ![Login](./src/main/resources/com/attendance/plus/attendanceplus/images/screenshots/Login.png) | ![Reminders](./src/main/resources/com/attendance/plus/attendanceplus/images/screenshots/Reminders.png) |
| :--------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
|                                          Login Screen                                          |                                            Reminders Panel                                             |

## Tech Stack

- **Java 24** (with preview features enabled)
- **JavaFX 17.0.6** - UI framework
- **Maven** - Build tool
- **JUnit 5** - Testing framework

## Prerequisites

- JDK 24 or higher
- Maven 3.6+

## Getting Started

### Clone the repository

```bash
git clone https://github.com/itsmeEVIL/AttendancePlus.git
cd AttendancePlus
```

### Run the application

```bash
./mvnw clean javafx:run
```

Or on Windows:

```cmd
mvnw.cmd clean javafx:run
```

## Project Structure

```
src/main/java/com/attendance/plus/attendanceplus/
├── AttendancePlus.java        # Main application entry point
├── LoginController.java       # Handles login/signup logic
├── DashboardController.java   # Main dashboard orchestration
├── MainPanelController.java   # Calendar navigation and display
├── SidePanelController.java   # Subject cards and attendance marking
├── TopBarController.java      # Top navigation bar
├── RemindersController.java   # Reminders popup window
└── LoginException.java        # Custom exception for login errors

src/main/resources/.../
├── fxml/                      # FXML layout files
├── styles/                    # CSS stylesheets
├── fonts/                     # Custom Inter font family
└── images/                    # App icons and screenshots
```

## Usage

1. **Sign Up** - Create a new account with username and password
2. **Login** - Enter credentials to access the dashboard
3. **Navigate Calendar** - Use arrow buttons to browse months, click a date to select it
4. **View Schedule** - The side panel shows classes scheduled for the selected date
5. **Mark Attendance** - Click "Attend" button on current day to mark yourself present
6. **View Stats** - Click on a subject card to expand and view attendance statistics
