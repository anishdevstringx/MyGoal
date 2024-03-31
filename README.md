# MyGoal
 This repo hosts a complete online banking project with source code and XAMPP for local deployment. Installation steps are in the README. Also included is a Robot Framework-based testing framework, aiding in creating robust test suites. Perfect for development and testing.

# How can you setup your project in local server using xampp 
To set up a project with XAMPP on your system and access it via localhost, follow these steps:

XAMPP Installation:

First, download the XAMPP installer from the Apache Friends website.
Open the downloaded file and install XAMPP on your system.
Starting XAMPP Control Panel:

Open the XAMPP control panel.
Start the Apache and MySQL services. This will activate your local server.
Placing Your Project Folder in XAMPP's 'htdocs' Directory:

Locate the 'htdocs' folder within your XAMPP installation directory. This folder serves as the root directory for XAMPP.
Copy or move your project folder into the 'htdocs' directory.
Database Setup (If Required):

Open localhost/phpmyadmin in your browser.
Use phpMyAdmin to create a new database for your project. If your project includes a database file (such as a .sql file), import that file here.
Project Configuration (If Required):

If your project connects to a database, you may need to update the database connection details (like database name, username, password) in your project's configuration files.
These details are usually found in a config.php file or a similar file within your project.
Accessing Your Project via Localhost:

Type localhost/your_project_folder_name in any web browser, where 'your_project_folder_name' is the name of your project folder within 'htdocs'.
Press Enter, and your project should open in the browser.

# How can you integrate your project with jenkins with local server
Setting up Jenkins locally for running on localhost involves downloading and executing the Jenkins WAR (Web Application Archive) file. Here are the steps to set up Jenkins locally:

Prerequisites
Java: Ensure you have Java (JRE or JDK) installed on your system because Jenkins is a Java-based application. You can check this by running java -version in your command line or terminal.
Steps to Set Up Jenkins
Download Jenkins:

Go to the official Jenkins website and navigate to the 'Download' section.
Download the latest stable Jenkins WAR file.
Run Jenkins:

Open your command line or terminal.
Navigate to the directory where you've downloaded the Jenkins WAR file.
Execute the following command to start Jenkins:
css
Copy code
java -jar jenkins.war --httpPort=8080
This command runs Jenkins on port 8080. You can change 8080 to any other port if you want Jenkins to run on a different port.
Access Jenkins:

Open a web browser and go to http://localhost:8080. You should see the Jenkins setup wizard starting.
Unlock Jenkins:

The first time you access Jenkins, it will ask you to "Unlock Jenkins" using an administrator password.
Locate the initial admin password in the console logs of your command line or terminal. The path to the password file will be displayed there.
Copy that password and paste it into the Jenkins setup wizard to unlock Jenkins.
Install Plugins:

After unlocking Jenkins, you'll be prompted to install plugins. You can choose to install suggested plugins or select specific plugins manually.
Create Admin User:

Once the plugins are installed, the next step is to create an admin user. Fill in the details and continue.
Jenkins URL:

The next screen will ask you to confirm the Jenkins URL. The default will be http://localhost:8080/. You can change this if needed, but the default should be fine for local setups.
Finish Setup:

After configuring the URL, click on "Start using Jenkins". You'll be taken to the Jenkins dashboard.
