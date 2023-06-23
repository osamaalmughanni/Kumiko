# What is Kumiko?
Kumiko is similar to the traditional Dynamo Player, as it enables you to execute your Dynamo scripts within Revit files. However, it goes beyond standard functionalities by offering enhanced portability, Git-based collaboration, and seamless script sharing among team members.

## Requirements
The app is designed for Windows-based computers and is distributed as a single executable (exe) file. Here are the key requirements:

- Operating System: Windows 10 or newer
- .NET Framework: Version 4.7.2 or newer
- Revit: Version 2013.1 or newer
- Git (Optional)

---

# Getting Started

## 1 — Get the latest version

Visit [getkumiko.com](https://www.getkumiko.com) to download the latest version of Kumiko. Make sure to close all active Revit applications and ensure that no Revit processes are running. After downloading the `Kumiko.exe` file, run it and follow the verification process.

## 2 — Verify your identity

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

Enter your email to verify your identity. Once logged in, please check your email for the verification code. Remember to check your junk mail folder if you don't receive any email. Enter or paste the code to access your account. The verification code will expire after 10 minutes.

## 3 — Organise your scripts

### 3.1 Kumiko's folder structure

By default, the recommended location for storing your Dynamo scripts is located at:
```
%USERPROFILE%\Kumiko
```
*You can also navigate to the root folder by clicking on the Kumiko logo in the sidebar.*

Dynamo scripts must be grouped within folders, with the folder name providing a description of the script's purpose. Here's an illustrative example of how you can organize your Dynamo scripts within the root directory.

```
- 📁 Kumiko
  ├── 📁 Export Room Areas
  │     └── 📄 script.dyn
  ├── 📁 Create Floor Plans
  │     └── 📄 script.dyn
  └── 📁 Generate 3D Views
        └── 📄 script.dyn
```

### 3.2 Playlists

You can also include multiple scripts within a folder if you want to run them sequentially as a Playlist:

```
- 📁 Kumiko
  ├── 📁 Export Room Areas
  │     ├── 📄 01-removeUnplaced.dyn
  │     └── 📄 02-saveToExcel.dyn
  ├── 📁 Create Floor Plans
  │     ├── 📄 01-renameViews.dyn
  │     └── 📄 02-createFloorPlans.dyn
  └── 📁 Generate 3D Views
        ├── 📄 01-adaptBoundingBox.dyn
        └── 📄 02-generateViews.dyn
```

When running multiple scripts, the execution order will depend on the alphabetical order. So, make sure to keep that in mind while organizing your scripts.

### 3.3 Document your script (Optional)

Additionally, you can include a `script.json` file to provide additional information about the script.

```
- 📁 Kumiko
  ├── 📁 Export Room Areas
  │   ├── 📄 01-removeUnplaced.dyn
  │   ├── 📄 02-saveToExcel.dyn
  │   └── 📝 script.json
  ├── 📁 Create Floor Plans
  │   ├── 📄 01-renameViews.dyn
  │   ├── 📄 02-createFloorPlans.dyn
  │   └── 📝 script.json
  └── 📁 Generate 3D Views
      ├── 📄 01-adaptBoundingBox.dyn
      ├── 📄 02-generateViews.dyn
      └── 📝 script.json
```

Here is a sample content of the `script.json` file:

```json
{
   "title":"Export Room Areas",
   "description":"Removes all unplaced rooms and saves all room areas to an excel file.",
   "author":"John Doe",
   "compatibility":"Revit 2022-2023",
   "dependencies":[
      "Clockwork",
      "BimorphNodes"
   ],
   "documentation":"https://github.com/johndoe/dynamo/blob/main/scripts/export_room_areas.md",
   "video":"https://www.youtube.com/watch?v=Nd6U2KgHI6k",
   "notes":"Please ensure you have the required packages installed: Clockwork and BimorphNodes."
}
```

The content of the `script.json` file will be displayed as badges in the script card in Kumiko.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.*

## 4 — Publish and run your scripts

Once you have successfully organized all your scripts, you can make them accessible by clicking on the synchronization symbol located in the sidebar. Once the symbol changes to green, your scripts will become visible and ready to be accessed or shared.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Sed diam voluptua. Eirmod tempor invidunt ut labore et dolore magna aliquyam erat*

## 5 — Connect to Git repository

Syncing your content with a remote Git repository offers several advantages. It provides convenient access to your work, promotes collaboration with fellow contributors, and enables efficient tracking of modifications.

### 5.1 Install Git

Kumiko requires Git to be installed in order to interact with your repository.

To install the latest version of Git on Windows, follow these steps:

1. Visit the official Git website: [https://git-scm.com/downloads](https://git-scm.com/downloads).
2. Download the installer for Windows.
3. Run the downloaded installer.
4. Follow the installation instructions, keeping the default settings unless you have specific preferences.
5. Complete the installation.

### 5.2 Edit the configuration file

To customize Kumiko's behavior, you can modify the `config.json` file.

1. Close Kumiko.
2. Locate the `config.json` file at `%LOCALAPPDATA%\Kumiko`.
3. Open the file in a text editor.
4. Find the `gitUrl` key and replace its value with the URL of your Git repository.
5. Save the changes.

Example `config.json`:

```json
{
  "rootDirectory": "C:\\Users\\John\\Kumiko",
  "gitUrl": "https://github.com/johndoe/dynamo.git",
  "windowWidth": 380.0,
  "windowHeight": 990.0,
  "windowTopPosition": 247.0,
  "windowLeftPosition": 1932.0,
  "windowTopMost": true
}
```

Now, Kumiko will automatically push content changes to the specified Git repository during synchronization if the `gitUrl` value is provided.

### 5.3 Git authentication

When synchronizing, you may be prompted to authenticate your Git credentials. Make sure to follow the provided authentication process or instructions to securely verify your Git credentials and enable any interaction between Kumiko and the Git repository.

## 6 — Manage Team Members

If you are a BIM Manager within an organization or company, there might be a need to share your scripts with other team members while maintaining control over their access to the content. In such circumstances, you have the option to grant other Members the ability to execute specific scripts and live access your latest content.

### 6.1 Add team members

To add Team members, click on the `team` page on the sidebar and follow the steps shown in this video

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.*

---

## Frequently Asked Questions

### Q: What is the purpose of this project?
A: Kumiko is a passion project developed by Osama Almughanni. Its main purpose is to simplify the process of developing, sharing, and version-controlling Dynamo scripts.

### Q: Can I use Kumiko for free?
A: Yes, absolutely. You can use most of Kumiko's features at no cost. However, you won't be able to add team members or share scripts without a paid subscription.

### Q: Does Kumiko detect uninstalled Dynamo packages?
A: Kumiko detects uninstalled Dynamo packages and notifies the user. However, the tool does not automatically install the missing packages. We are working on implementing auto-installation options in the future.

### Q: Does Kumiko detect input nodes?
A: Yes, Kumiko detects automatically input nodes and prompts the user to modify the inputs before executing the script. Please notice that there may be some input types that are not currently supported. 

### Q: How can I report an issue or suggest a new feature?
A: We currently do not have a platform to manage different requests, so please send us an email at mail@getkumiko.com, and we will be glad to help.

---

## License

This project is released under the terms of the End-User License Agreement (EULA).

Please carefully read and understand the terms and conditions outlined in the EULA before using or contributing to this project.

You can find the full text of the EULA <a href="https://getkumiko.com/eula" target="_blank">Here</a>.
