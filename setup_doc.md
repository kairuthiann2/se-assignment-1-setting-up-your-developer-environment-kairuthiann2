My step-by-step processes for dev set up

# Install Windows 11

Step 1

Check System Requirements:

Make sure your PC meets the minimum requirements for Windows 11:
Processor: 1 GHz or faster with 2 or more cores on a compatible 64-bit processor or System on a Chip (SoC).
RAM: 4 GB or more.
Storage: 64 GB or larger storage device.
Firmware: UEFI, Secure Boot capable.
TPM: Trusted Platform Module (TPM) version 2.0.
Graphics card: DirectX 12 compatible graphics / WDDM 2.x.
Display: >9” with HD Resolution (720p).

Step 2

Download Windows 11

Go to the Windows 11 download page and click on "Download now" to get the Installation Assistant.

Step 3

Open the downloaded Installation Assistant and follow the on-screen instructions to upgrade or install Windows 11.

Step 4

Follow the on-screen prompts to complete the Windows 11 setup, including language, region, and user account setup.

# Install Visual Studio Code

Step 1

Visit the Visual Studio Code download page.

Step 2

Download the installer for Windows. Run the `.exe` file to start the installation process.

Step 3

Follow the installation wizard, and select the options to add VS Code to your PATH and create a desktop shortcut.

Step 4

After installation, open Visual Studio Code from the Start menu or desktop shortcut.

# Installation of Python

Step 1 Download Python Installer

Open your web browser and go to the official Python download page.

On the download page, click the "Download Python" button. This will download the latest version of Python for Windows.

Step 2 Run the Python Installer

Locate the downloaded file (e.g., `python-3.x.x.exe` where `3.x.x ` is the version number) and double-click to run it.

A setup window will appear. Make sure to check the box that says "Add Python to PATH". This will make it easier to run Python from the command line.

Click on "Install Now".

If you want to customize the installation, click on "Customize installation". Here you can choose additional features, the installation location, and advanced options.

Step 3 Complete the Installation

The installer will now copy files and set up Python on your system. This might take a few minutes.

Once the installation is complete, you will see a "Setup was successful" message. You can close the installer window.

Step 4 Verify the Installation

Press `Win + R`, type `cmd`, and press `Enter` to open the Command Prompt.

In the Command Prompt, type `python --version` and press `Enter`. You should see the installed Python version number displayed (e.g., `Python 3.x.x`).

PIP is the package installer for Python, and it gets installed automatically with Python. To verify, type `pip --version` and press `Enter`. You should see the PIP version number displayed.

# Installation of MySQL

Step 1 Download MySQL Installer:

Go to the MySQL Community Server download page.

Select the Windows (x86, 64-bit) version and download the MySQL Installer.

Step 2 Run the Installer

Open the downloaded `.msi` file to start the installation.

Step 3 Choose Setup Type

Select "Developer Default" to install MySQL Server, MySQL Workbench, and other tools.

Step 4 Configure MySQL Server

Follow the setup wizard to configure MySQL Server. Set the root password and choose the server configuration options.

Step 5 Complete Installation
Finish the installation and launch MySQL Workbench or MySQL Shell from the Start menu.

# Installation of Dart SDK

Step 1 Download Dart SDK:

Visit the Dart SDK page.

Step 2 Download the Windows SDK:

Click on "Download Dart SDK" and save the `.zip` file.

Step 3 Extract the SDK:

Extract the contents of the `.zip` file to a folder of your choice, e.g., `C:\dart`. Use 7zip free version for the extraction.

Step 4 Set up the Environment Variables:

Open System Properties and go to Advanced System Settings.
Click on Environment Variables.
Under System Variables, find Path and click Edit. Add the path to the Dart SDK's `bin` directory, e.g., `C:\dart\dart-sdk\bin`.

Step 5 Verify Dart Installation:

Open Command Prompt and type `dart --version` to verify the installation.

# Installion of Flutter

Step 1 Download Flutter SDK

Go to the Flutter SDK download page.

Download the Flutter SDK `.zip` file.

Step 2 Extract the Flutter SDK

Extract the `.zip` file to a location of your choice, e.g., `C:\flutter` using the 7zip file extractor.

Step 3 Set up Environment Variable

Open System Properties and go to Advanced System Settings.

Click on Environment Variables.

Under System Variables, find Path and click Edit. Add the path to the Flutter SDK’s `bin` directory, e.g., `C:\flutter\bin`.

Step 4 Run Flutter Doctor:

Open Command Prompt and type` flutter doctor` to check for any dependencies that need to be installed.

Step 5 Install Android Studio (Optional but Recommended):

Download and install Android Studio from the Android Studio website.
During installation, make sure to install the Android SDK, Android Virtual Device (AVD), and Flutter plugin.

Step 6 Verify Flutter Installation:

Run `flutter doctor` again to ensure that everything is set up correctly.

# customizations made with screenshots

while installing the MySQL select `customize` instead of the `server option` in the Choose `set up type`. Click `next`

Under `select product` select the server version. By default it will be selected for you.

Since you choose Customize in the `set up type` now you can select the `Application` you would like to have .

In my case i choose MySQL `workbench` and MySQL `shell`

# A reflection on the challenges faced during setup and strategies employed to overcome them.

1.  Issues Encountered with MySQL installation process

- Denied access for root@localhost with password 'root'

Troubleshooting Steps for This Issue(used a guide from a youtube tutorial video by `Amit Thinks ` and `KaRam` )

step 1
uninstall MySQL completely from your PC.

step 2
Restart your PC.

step 3
Reinstall MySQL once again.

step 4
This time set a new password.

step 5
Ensure the path is set to the system variables and the user variables.

step 6
Then run MySQL -u root -p and enter your password to access MySQL server.

step 7
Now start on creating your database.
