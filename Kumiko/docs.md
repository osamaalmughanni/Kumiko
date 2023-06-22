# What is Kumiko?
Kumiko is similar to the traditional Dynamo Player, as it allows you to run your Dynamo scripts inside Revit files. However, it surpasses standard functionalities by providing enhanced portability, a version-controlled collaboration with git and easy script sharing with other members.

## Requirements
The app is designed to operate exclusively on Windows-based computers. It is developed as a single executable (exe) file, meaning that it encompasses all the necessary code and resources for execution. However, there are some key requirements that should be considered, these are:

- Windows 10 or greater
- .NET Framework 4.7.2 or greater
- Revit 2013.1 or greater
- git (Optional)

---

# Getting Started

## 1 Get the latest version

Download the latest version of Kumiko from [getkumiko.com](https://www.getkumiko.com), close all active Revit applications, and ensure that no Revit processes are running. Run the downloaded Kumiko.exe file and proceed with the verification process.

## 2 Verify your identity

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

First, enter your email to verify your identity. After logging in, check your email for the verification code. Remember to check your junk mail folder if you don't recieve any email. Enter or paste the code to access your account. The verification code will expire after 10 minutes.

## 3 Organise your scripts

### 3.1 Understand the folder structure

By default, the recommended location for storing your Dynamo scripts is located at:
```
%USERPROFILE%\Kumiko
```
*You can also navigate to the root folder by clicking on the Kumiko logo in the sidebar.*

Dynamo scripts must be grouped within folders, with the folder name providing a description of the script's purpose. Here's an illustrative example of how you can organize your Dynamo scripts within the root directory.

```
- 📁 Kumiko
  ├── 📁 Extract Room Areas
  │     └── 📄 script.dyn
  ├── 📁 Create Floor Plans
  │     └── 📄 script.dyn
  └── 📁 Generate 3D Views
        └── 📄 script.dyn
```

### 3.2 Add Playlists

You can also include multiple scripts within a folder if you want to run them sequentially:

```
- 📁 Kumiko
  ├── 📁 Extract Room Areas
  │     ├── 📄 01-updateValues.dyn
  │     └── 📄 02-saveToExcel.dyn
  ├── 📁 Create Floor Plans
  │     ├── 📄 01-renameViews.dyn
  │     └── 📄 02-createFloorPlans.dyn
  └── 📁 Generate 3D Views
        ├── 📄 01-adaptBoundingBox.dyn
        └── 📄 02-generateViews.dyn
```

When running multiple scripts within a folder, their execution order will be influenced by their alphabetical order. So, make sure to keep that in mind while organizing your scripts.

### 3.3 Document your script (Optional)

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

The json content will be then visualised as badges inside the script.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.*

## 4 Publish your scripts

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

### 4.1 Run your first script

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

## 5 Connecting to Git repository (Optional)

### 5.1 Edit the configuration file

To personalize Kumiko's behavior and adapt it to your specific needs and preferences, you can make changes to the `config.json` file.

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

Here is a short explanation for each setting:

1. `rootDirectory`: Storage folder for Kumiko's files and data.
2. `gitUrl`: URL of the Git repository Kumiko syncs with.
3. `windowWidth` and `windowHeight`: Dimensions of Kumiko's application window.
4. `windowTopPosition` and `windowLeftPosition`: Position of Kumiko's window on the screen.
5. `windowTopMost`: Boolean for keeping Kumiko's window always on top.

### 5.2 Git authentication

When working with Git, you may be prompted to authenticate your Git credentials. Make sure to follow the provided authentication process or instructions to securely verify your Git credentials and enable any interaction between Kumiko and the Git repository.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.*

## 6 Manage Team Members

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 

### 6.1 Add team members
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
