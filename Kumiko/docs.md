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

## 01 Get the latest version

Download the latest version of Kumiko, close all active Revit applications, and ensure that no Revit processes are running. Run Kumiko and start the verification process.

## 02 Verify your identity

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

Our login process is passwordless. Upon logging in, you will receive a verification code via email. This code is valid for 10 minutes. Simply enter or paste the code into Kumiko to access your account.

## 03 Add your first script

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

The default root folder is located at:
```
%LOCALAPPDATA%\Kumiko
```

---

# Configuration
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
