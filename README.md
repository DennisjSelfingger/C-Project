# C-Project
Week 8 Project
This Password Manager is a simple C++ console application designed to securely store and manage passwords for various websites or services. It allows users to add new passwords, retrieve existing passwords, and list all stored passwords. Additionally, it offers the option to generate random, secure passwords. 
  This application is a basic demonstration and does not include encryption or other advanced security features, so please do not count on this to secure any of your private password, again just an example program!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

Features
Add Passwords: Save passwords associated with specific sites.
Generate Random Passwords: Securely generate and store a random password.
Retrieve Passwords: Look up the password for a particular site.
List Passwords: Display all stored site-password pairs.
Simple Console Interface: Easy-to-use text-based interface.
How to Use
Start the Application: Run the program in a console or terminal.
Add a New Password:
The application will first ask if you want to add a new password. Reply with 'y' (yes) or 'n' (no).
If you choose 'y', you will be prompted to enter the name of the site.
Next, you can choose to generate a random password or enter your own.
To generate a random password, reply with 'y' when asked. The application will generate a secure password for you and display it.
To enter your own password, reply with 'n' and then type your password.
The application will confirm that the password has been successfully saved.
Retrieve a Password:
To retrieve a password, use the getPassword function in the code. (Note: This functionality is currently available only within the code and not through the console interface.)
List All Passwords:
To see all stored passwords, the application will list them out after adding a new password. Each site-password pair is displayed.
Exit the Application:
The application will close after pressing any key when prompted, or you can manually close the console window.

EXAMPLE 
Do you want to add a new password? (y/n): y
Enter the site name: example.com
Do you want to generate a random password? (y/n): y
Generated password: X7gfa#4!0sKm
Password added successfully!
Password saved.

example.com: X7gfa#4!0sKm
