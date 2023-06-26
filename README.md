# What is Kumiko?
Kumiko is similar to the traditional Dynamo Player, as it enables you to execute your Dynamo scripts within Revit files. However, it goes beyond standard functionalities by offering enhanced portability, Git-based collaboration, and seamless script sharing among team members.

https://github.com/osamaalmughanni/Kumiko/assets/49910802/d3a58a2d-9325-49d6-bb5e-171b8116f20e

## Requirements
The app is designed for Windows-based computers and is distributed as a single executable (exe) file. Here are the key requirements:

- Operating System: Windows 10 or newer
- .NET Framework: Version 4.7.2 or newer
- Revit: Version 2013.1 or newer
- Git (Optional)

---

# Getting Started

## 1 — Get the Latest Version

Visit [getkumiko.com](https://www.getkumiko.com) to download the latest version of app. Make sure to close all active Revit applications and ensure that no Revit processes are running. After downloading the `Kumiko.exe` file, run it and follow the verification process.

## 2 — Verify Your Identity

Enter your email to verify your identity. Once logged in, please check your email for the verification code. Remember to check your junk mail folder if you don't receive any email. Enter or paste the code to access your account. The verification code will expire after 10 minutes.

https://github.com/osamaalmughanni/docs/assets/49910802/deeaad56-3074-4c62-b75f-c6eadb8677ac

*Kumiko operates as a webview and is dependent on an internet connection for its functionality.*

---

# Usage

## 3 — Organise Your Scripts

### 3.1 Folder Structure

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

### 3.3 Metadata (Optional)

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
   "notes":"Please ensure you have the required packages installed: Clockwork and BimorphNodes."
}
```

The content of the `script.json` file will be displayed as badges inside Kumiko.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*The documentation badge is interactive and, when clicked, will redirect the user to the provided URL.*

## 4 — Publish Your Scripts

Once you have successfully organized all your scripts, you can make them accessible by clicking on the synchronization symbol located in the sidebar. Once the symbol changes to green, your scripts will become ready to be accessed or shared.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*After synchronizing your content, your scripts will be ready to execute within Revit. Simply hover the mouse over the script and click the Play button.*

## 5 — Connect to Repository (Optional)

Connecting your content to a remote Git repository offers various benefits, including convenient access, collaboration with others, and efficient tracking of modifications.

To interact with your repository using Kumiko, please follow these steps:

### 5.1 Install Git

1. Visit the official Git website: https://git-scm.com/downloads.
2. Download the installer for Windows.
3. Run the downloaded installer.
4. Follow the installation instructions, sticking to the default settings unless you have specific preferences.
5. Complete the installation process.

### 5.2 Edit Configuration File

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

Now, Kumiko will automatically fetch and apply content changes to the designated Git repository during synchronization.

### 5.3 Git Authentication

When synchronizing, you may be prompted to authenticate your Git credentials. Make sure to follow the provided authentication process or instructions to securely verify your Git credentials and enable any interaction between Kumiko and the Git repository.

## 6 — Manage Team Members

If you are a BIM Manager within an organization or company, there might be a need to share your scripts with other team members while maintaining control over their access to the content. In such circumstances, you have the option to grant other Members the ability to instantly access your latest content upon synchronising.

### 6.1 Add Team Members to all Resources

To share all your scripts with specific team members, click on the "Team" page in the sidebar and follow the steps demonstrated in this video.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Team members will not be able to view the content of your script; they will only be able to execute it.*

### 6.2 Add Team Members to Specific Resources

To control which resources team members can access, you must first organize your scripts using a more structured approach. Start by creating a main folder for each project or category and put the relevant scripts inside. This way, you can assign team members to specific projects, allowing them access only to the resources within their assigned project.

Here's an example on how organize your scripts based on projects:

```
- 📁 Kumiko
  ├── 📁 Project A
  │     ├── 📁 Export Room Areas
  │     │     ├── 📄 01-removeUnplaced.dyn
  │     │     └── 📄 02-saveToExcel.dyn
  │     ├── 📁 Create Floor Plans
  │     │     ├── 📄 01-renameViews.dyn
  │     │     └── 📄 02-createFloorPlans.dyn
  │     └── 📁 Generate 3D Views
  │           ├── 📄 01-adaptBoundingBox.dyn
  │           └── 📄 02-generateViews.dyn
  ├── 📁 Project B
  │     ├── .
  │     └── .
  └── 📁 Project C
        ├── .
        └── .
```

In this case, you can add a team member to the resource `Project A` and share only the scripts within that folder.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

You can also be more specific by using a forward slash. For example: `Project A/Export Room Areas.`

## 7 — Featured Scripts

With Kumiko, we strive to share high-quality and dependency-free scripts within our community. You can explore our featured scripts by visiting the Featured page and give them a try. If you would like to feature one of your scripts with Kumiko, please get in touch with us via email.

https://github.com/osamaalmughanni/docs/assets/49910802/dfb060e5-15e3-436a-a298-0140d0f220c6

*Click on the documentation badge to read the documentation and better understand the functionality of each script.*

---

## Frequently Asked Questions

### Q: What is the purpose of this project?
A: Kumiko's main purpose is to simplify the process of developing, sharing, and version-controlling Dynamo scripts.

### Q: Can I use Kumiko for free?
A: Yes, absolutely. You can use most of Kumiko's features at no cost. However, you won't be able to add team members or share scripts without a paid subscription.

### Q: Does Kumiko detect uninstalled Dynamo packages?
A: Kumiko detects uninstalled Dynamo packages and notifies the user. However, it will not automatically install the missing packages. We are working on implementing auto-installation options in the future.

### Q: Does Kumiko detect input nodes?
A: Yes, Kumiko detects automatically input nodes and prompts the user to modify the inputs before executing the script. Please notice that there may be some input types that are not yet supported.

---

## Contribution

We value your feedback and encourage you to <a href="https://github.com/osamaalmughanni/Kumiko/issues/new" target="_blank">open an issue</a> to dicuss any major changes. Your input is important to us, as it helps us address concerns and incorporate suggestions.

If you enjoy using Kumiko, consider making a <a href="https://liberapay.com/osamaalmughanni/donate" target="_blank">donation</a> or support us by subscribing to our premium plans.

---

## License

This project is released under the terms of the End-User License Agreement (EULA). Please carefully read and understand the terms and conditions outlined in the EULA before using the app. You can find the full text of the EULA <a href="https://getkumiko.com/eula" target="_blank">here</a>.

© 2023 Kumiko
