# Overview
Kumiko is similar to the traditional Dynamo Player, as it allows you to run your Dynamo scripts. However, it surpasses standard functionalities by providing enhanced portability, a version-controlled collaboration with git and easy script sharing with other members.

## Requirements
Kumiko is designed to operate exclusively on Windows-based computers. It has been developed as a single executable (exe) file, meaning that it encompasses all the necessary code and resources for execution. Here are some key requirements:

- Windows 10 or greater
- .NET Framework 4.7.2 or greater
- Revit 2013.1 or greater
- git (Optional)

---

# Getting Started

## 1 Get the latest version

Download the latest version of Kumiko from [getkumiko.com](https://www.getkumiko.com), close all active Revit applications, and ensure that no Revit processes are running. Run the downloaded Kumiko.exe file and proceed with the verification process.

After running, Kumiko will detect any Revit version (2023.1 or later) and automatically install the necessary .dll and .addin files for you.

## 2 Verify your identity

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

Enter your email to verify your identity. After logging in, check your email for a verification code. Remember to check your junk mail folder if you don't see the email. The code will expire after 10 minutes. Enter or paste the code to access your account.

## 3 Publish your first script

### 3.1 Kumiko's root folder

By default, the recommended location for storing your Dynamo scripts is located at:
```
%USERPROFILE%\Kumiko
```

This is an example on how you can organise your Dynamo scripts:

```
- 📁 Extract Room Areas
  └── 📄 script.dyn
- 📁 Create Floor Plans
  └── 📄 script.dyn
- 📁 Generate 3D Views
  └── 📄 script.dyn
```

```
- 📁 Extract Room Areas
  ├── 📄 script.dyn
  └── 📄 script.json 🗎

- 📁 Create Floor Plans
  ├── 📄 script.dyn
  └── 📄 script.json 🗎

- 📁 Generate 3D Views
  ├── 📄 script.dyn
  └── 📄 script.json 🗎
```

### 3.2 Sync
At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

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

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

## 5 Add team members
At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

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
