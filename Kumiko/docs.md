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

Enter your email to verify your identity. After logging in, check your email for a verification code. Remember to check your junk mail folder if you don't recieve the email. The code will expire after 10 minutes. Enter or paste the code to access your account.

# 3 Publish your first script

## 3.1 Understand Kumiko's folder structure

By default, the recommended location for storing your Dynamo scripts is located at:
```
%USERPROFILE%\Kumiko
```

Dynamo scripts are organised inside folders. The folder name describes basically what the script does, while the file name itself isn't as relevant.
This is an example on how you can organise your Dynamo scripts inside the root directory:

```
- 📁 Kumiko
  ├── 📁 Extract Room Areas
  │     └── 📄 script.dyn
  ├── 📁 Create Floor Plans
  │     └── 📄 script.dyn
  └── 📁 Generate 3D Views
        └── 📄 script.dyn
```

### 3.1.1 Playlists

You can also include multiple scripts within a folder if you want to run them sequentially:

```
- 📁 Kumiko
  ├── 📁 Extract Room Areas
  │     ├── 📄 updateValues.dyn
  │     └── 📄 saveToExcel.dyn
  ├── 📁 Create Floor Plans
  │     ├── 📄 renameViews.dyn
  │     └── 📄 createFloorPlans.dyn
  └── 📁 Generate 3D Views
        ├── 📄 adaptBoundingBox.dyn
        └── 📄 generateViews.dyn
```

### 3.1.2 Script Documentation

Additionally, you can include a `script.json` file to provide additional information about the script.

```
- 📁 Kumiko
  ├── 📁 Extract Room Areas
  │   ├── 📄 updateValues.dyn
  │   ├── 📄 saveToExcel.dyn
  │   └── 📄 script.json
  ├── 📁 Create Floor Plans
  │   ├── 📄 renameViews.dyn
  │   ├── 📄 createFloorPlans.dyn
  │   └── 📄 script.json
  └── 📁 Generate 3D Views
      ├── 📄 adaptBoundingBox.dyn
      ├── 📄 generateViews.dyn
      └── 📄 script.json
```

This is an example of how such a file might look like.

```json
{
   "title":"Export data as .xlsx",
   "description":"Export an active open schedule with element IDs from Revit to Excel, facilitating data analysis and manipulation outside of Revit.",
   "author":"Osama Almughanni",
   "compatibility":"Revit 2022-2023",
   "dependencies":[
      "Clockwork",
      "BimorphNodes"
   ],
   "documentation":"https://example.com/script-documentation",
   "video":"https://www.youtube.com/watch?v=Nd6U2KgHI6k",
   "notes":"Please ensure you have the required packages installed: Clockwork and BimorphNodes."
}
```

### 3.1.3 Sync your scripts

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

# 4 Connecting to your remote Git repository

## 4.1 Configurate

To personalize Kumiko's behavior and adapt it to your specific needs and preferences, you can make changes to the `config.json` file. Follow the steps below to edit the configuration file:

1. Close Kumiko to ensure that any modifications can take effect.
2. Locate the `config.json` file in the following directory:

```
%LOCALAPPDATA%\Kumiko
```

3. Open the config.json file using a text editor of your choice.

Inside the config.json file, you will find various settings that you can customize. Here is an example of the file's structure:

```json
{
  "rootDirectory": "C:\\Users\\[username]\\Kumiko",
  "gitUrl": "https://github.com/[username]/[repo].git",
  "windowWidth": 380.0,
  "windowHeight": 990.0,
  "windowTopPosition": 247.0,
  "windowLeftPosition": 1932.0,
  "windowTopMost": true
}
```

Here is a brief explanation for each setting:

**rootDirectory**: Specifies the root directory where Kumiko will store its files and data. You can modify this path to a directory of your choice.

**gitUrl**: Specifies the URL of the Git repository that Kumiko will sync with. You can change this setting to sync Kumiko with your Git repository.

**windowWidth** and **windowHeight**: Determine the dimensions of Kumiko's application window. You can adjust these values to suit your screen size and personal preference.

**windowTopPosition** and **windowLeftPosition**: Control the position of Kumiko's window on your screen. You can modify these values to change its default placement.

**windowTopMost**: A boolean value that determines whether Kumiko's window will always stay on top of other windows. Set it to `true` if you want Kumiko's window to be topmost; otherwise, set it to `false`.

## 4.2 Add Git credentials

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita `config.json` gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

# 5 Collaboration

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

## 5.1 Add team members
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
