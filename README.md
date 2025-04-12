LocationFinder App
This is a full-stack application that allows users to:
- Lookup IP geolocation information.
- Store and retrieve IP address records efficiently.
- Avoid duplicate IP entries in the database.
- Provide a clean and usable frontend interface.

Features
- IP Geolocation Lookup: Fetch geolocation data for a given IP address.
- Efficient Storage: Store IP address records inSqlite database and prevent duplicates.
- Error Handling: Gracefully handle invalid IPs and failed external API calls.
- Frontend UI: Interactive and user-friendly interface styled with Android Studio resource files.


Endpoints
1. POST /fetch-ip
- Accepts an IP address.
- Checks if the IP address already exists in the database:- If exists, returns the stored data from database.
- If not, fetches data from ipinfo.io, stores it in sqlite database, and returns the response.

- Prevents duplicate entries in the database.

- 2. GET /stored-ips
- Returns a list of all stored IP address records from sqlite database.


Frontend Requirements
- Input field for users to enter an IP address.
- Display geolocation details, such as:- City
- Country
- Region
- ISP and map of the particular location
- List of all previously stored IP addresses and their geolocation details.
- Built using xml for a clean, responsive design.


How to Run with Android Studio
Prerequisites
- Android Studio (latest version).
- Internet access for fetching IP geolocation data from ipinfo.io.

Installation

1.clone this repository
git clone https://github.com/your-repo/ip-geolocation-app.git
cd ip-geolocation-app

2.Open Android Studio and import Project

Click File-> Open
Select the root Directory of the cloned project

3.Install Dependencies
Navigate to the project folder in the terminal
Install backend dependencies by running.
4.Start Frontend
5.Start Backend
6.Access the application
use an Android emulator in android studio to test the app

Tech Stack
Backend:
- Java
- Sqlite Database

Frontend:
Android Xml resource

External API:
- ipinfo.io

Error Handling
- Invalid IP Address: Users are notified if the entered IP is invalid.
- Failed API Calls: The app shows an error message if the external API call fails.
Core Requirements Fulfilled
   Prevents duplicate entries in the database.
   Provides a clean and usable UI.
   Handles errors gracefully.
   Efficient lookups before calling external APIs.
















