# Overview

Kumiko is similar to the traditional Dynamo Player, as it allows you to run your Dynamo scripts. However, it surpasses standard functionalities by providing enhanced portability, a version-controlled collaboration with git and easy script sharing with other members.

## Requirements
Kumiko is designed to operate exclusively on Windows-based computers. It has been developed as a single executable (exe) file, meaning that it encompasses all the necessary code and resources for execution. Here are however the main requirements:

- Windows 10 or greater
- .NET Framework 4.7.2 or greater
- Revit 2013.1 or greater
- git (Optional)

---

# Getting Started

## 1 Get the latest Kumiko version

Download the latest version of Kumiko from [getkumiko.com](https://www.getkumiko.com), close all active Revit applications, and ensure that no Revit processes are running. Run the downloaded Kumiko.exe file and proceed with the verification process.

## 2 Verify your identity

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

Our login process is passwordless. After logging in, please check your email for a verification code. If you don't receive the email, please remember to check your junk mail folder. The code will be valid for 10 minutes. Enter or paste the code to access your account.

## 3 Publish your first script

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

## 4 Connecting to your remote Git repository

### 4.1 Edit configuration file

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita `config.json` gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

The file can be found under:
```
%LOCALAPPDATA%\Kumiko
```

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

```json
{
  "rootDirectory": "C:\\Users\\osama\\Kumiko",
  "gitUrl": "https://github.com/osamaalmughanni/mydynamoscripts.git",
  "windowWidth": 380.0,
  "windowHeight": 990.0,
  "windowTopPosition": 247.0,
  "windowLeftPosition": 1932.0,
  "windowTopMost": true
}
```

### 4.2 Add Git credentials

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita `config.json` gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

### 4.3 Sync your scripts

---

# Frequently Asked Questions

### Q: What is the purpose of this project?
A: The purpose of this project is to create a user-friendly interface for managing tasks efficiently.

### Q: How can I install and run this project locally?
A: To install and run this project locally, follow these steps:
1. Clone the repository: `git clone https://github.com/your-username/your-repo.git`
2. Navigate to the project directory: `cd your-repo`
3. Install the dependencies: `npm install`
4. Start the development server: `npm start`

### Q: Are there any prerequisites to using this project?
A: Yes, there are a few prerequisites for using this project. You need to have Node.js and npm installed on your system. You can download them from the official Node.js website: [https://nodejs.org](https://nodejs.org)

### Q: Can I contribute to this project?
A: Absolutely! Contributions are welcome. Please fork the repository, make your changes, and submit a pull request. Don't forget to follow our contribution guidelines.

### Q: How can I report an issue or suggest a new feature?
A: If you encounter any issues or have suggestions for new features, please open an issue on the GitHub repository. We appreciate your feedback!

---
