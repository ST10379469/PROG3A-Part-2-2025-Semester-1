# PROG3A-Part-2-2025-Semester-1
Running the Application
Follow these steps to build and run the Agri-Energy Connect web application locally after completing the Installation and Database Setup steps.

Build the Project:

Open a terminal (or Command Prompt) and navigate to the project directory:cd C:\Users\kheni\source\repos\AgriEnergyConnect\AgriEnergyConnect


Build the project to compile the code and check for errors:dotnet build


If errors occur (e.g., "The type or namespace name 'LoginModel' could not be found"), see the Troubleshooting section.


Run the Application:

Start the application using the .NET CLI:dotnet run


Alternatively, in Visual Studio:
Open the solution: C:\Users\kheni\source\repos\AgriEnergyConnect\AgriEnergyConnect.sln.
Press F5 or click Start to run in Debug mode.


The application will start, and the terminal will display the URL (e.g., Now listening on: https://localhost:7184).
Note: The port may vary. Check Properties/launchSettings.json for the configured port (e.g., 7184).


Access the Web Interface:

Open a web browser and navigate to the URL shown in the terminal (e.g., https://localhost:7184).
You should see the Agri-Energy Connect homepage with Login and Register buttons in the navigation bar.


Test Authentication:

Register a New User:
Click Register (navigates to /Identity/Account/Register).
Enter details (e.g., Email: farmer@example.com, Password: Farmer123!, Confirm Password: Farmer123!).
Submit the form to create a user with the "Farmer" role.
Verify redirection to the Farmer dashboard (/Farmer/Dashboard).


Log In:
Click Login (navigates to /Identity/Account/Login).
Use an existing user (e.g., Email: admin@example.com, Password: Password123!) or the user created above.
Check the "Remember me" box (optional) and submit.
Verify redirection to the homepage or dashboard based on the user’s role.


Log Out:
Click Logout (if logged in) to sign out and return to the homepage.




Verify Functionality:

Ensure the Login and Register pages load without errors.
Confirm that registered users can access the Farmer dashboard.
If you encounter issues (e.g., 404 errors, validation script errors), see the Troubleshooting section.



Note: If you modify the code (e.g., Login.cshtml.cs, Register.cshtml.cs), rebuild the project (dotnet build) before running to apply changes.
