# C-Project
Week 8 Project

SUMMARIZE AND ANSWERS TO THESE QUESTIONS
Summarize the project and what problem it was solving.


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
To generate a random password, reply with 'y' when asked. The application will generate and display a secure password for you.
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


What did you do particularly well?

I think The implementation of the std::random_device and std::mt19937 for password generation was done particularly well. These components ensure that each generated password is random and secure, providing a significant level of unpredictability in the password creation process. This would make it harder for someone to figure out and find someone's maiden name, birthday, favorite pet ect. would have no effect on figuring out the password.

Where could you enhance your code?

 I could improve The code could be enhanced by adding encryption for stored passwords, maybe making it 64 bit instead of 32.   I could also add user authentication system before allowing access to stored passwords and include special characters, upper and lower case letter which would enhance the generator.

 Which pieces of the code did you find most challenging to write, and how did you overcome this?
 
Understanding and implementing the random number generation for password creation was the most challenging due to the complex nature of C++'s random library. Overcoming this challenge involved researching on Google and looking at documentation from encryption algorithms to see what was used most and available, along with watching YouTube and testing. Keeping track of the classes was a bit difficult; I just need to get used to it.


What tools or resources are you adding to your support network?

To support ongoing development, tools like version control systems (e.g., Git), I am trying to learn and get more familiar with. Also, command line scripting, bash, Linux, windows, and more familiar in error handling to catch bugs. I also am trying to learn the ins and outs of IDE's so I can use all the tools and extensions they have available to make life easier.


What skills from this project will be particularly transferable to other projects or coursework?

Skills such as object-oriented programming, data structure management, secure random number generation, and user input handling will be transferable to a wide range of future projects. These fundamental skills form the core of many programming tasks and are applicable to various types of software engineering. The main thing I have been getting used to, and I am getting better at it, is just structure. This really helps me to stay organized. I have always been very organized, but I have found out, at least for me, that organization is a little more of a learning curve than, say, organizing a sock drawer!

How did you make this program maintainable, readable, and adaptable?

The program was made maintainable and readable by using clear naming conventions, organizing code into classes and methods, and adding comments explaining the purpose and functionality of code sections.  I made the design more  adaptable through modular coding practices, allowing for easy updates or expansion of functionality, such as adding new features or changing how passwords are stored and retrieved.




HERE IS THE PSEUDOCODE
Program PasswordManager
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! Again, this is just a simple app, so please do not count on this for securing your passwords. It still needs work and better encryption.!!!!!!!!!!!!!!!!!

Class PasswordManager:
    Define passwords as a map of strings to strings

    Constructor PasswordManager:
        Initialize passwords

    Destructor PasswordManager:
        Clean up any resources if necessary

    Function addPassword(site, password):
        Try to add (site, password) to passwords
        Return true if added, false if site already exists

    Function removePassword(site):
        Remove the password for the given site
        Return true if removed, false if site does not exist

    Function getPassword(site):
        Return the password for the given site, or an empty string if not found

    Function listAll:
        Print all site-password pairs

    Function generatePassword(length):
        Generate a random password of the given length
        Return the generated password

Main Program:
    Create an instance of PasswordManager

    Ask the user if they want to add a new password
    If yes:
        Prompt for the site name
        Ask if the user wants to generate a random password
        If yes:
            Generate a random password and display it
        Else:
            Prompt the user to enter a password
        Add the password for the site
        Display a success or failure message

    Optionally, list all passwords

    End program
