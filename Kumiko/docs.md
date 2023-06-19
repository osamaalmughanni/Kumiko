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

## 01 Verification

![alt text](https://github.com/osamaalmughanni/docs/blob/main/Kumiko/links/redk.gif?raw=true)

Download the latest version of Kumiko, close all active Revit applications, and ensure that no Revit processes are running. Run Kumiko and start the verification process.

## 02 Connecting with git

The default root folder is located at:
```
%LOCALAPPDATA%\Kumiko
```

Here is an example of how the folder content can look like:

```
📁 Chairs
├── 📁 Eames Lounge Chair
│   ├── 📄 Eames Lounge Chair.ai
│   ├── 📄 Eames Lounge Chair.obj
│   └── 🌅 cover.jpg
├── 📁 Barcelona Chair
│   ├── 📄 Barcelona Chair.max
│   ├── 📄 Barcelona Chair.obj
│   └── 🌅 cover.jpg
└── 🌅 cover.jpg

📁 Tables
├── 📁 Eames Dining Table
│   ├── 📄 Eames Dining Table.rvt
│   ├── 📄 Eames Dining Table.obj
│   └── 🌅 cover.jpg
├── 📁 Tulip Table
│   ├── 📄 Tulip Table.dwg
│   ├── 📄 Tulip Table.obj
│   └── 🌅 cover.jpg
└── 🌅 cover.jpg
```

### Library

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.

```
📁 Library A
├── 📁 Object 1
│   ├── 📄 Object 1.ai
│   ├── 📄 Object 1.obj
│   └── 🌅 cover.jpg
├── 📁 Object 2
│   ├── 📄 Object 2.max
│   ├── 📄 Object 2.obj
│   └── 🌅 cover.jpg
├── 🌅 cover.jpg
└── 📄 library.json
```

Justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata `cover.jpg` sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, diam voluptua.

```
📁 Library
├── 📁 Object A
│   ├── 📄 Object A.ai
│   ├── 📄 Object A.obj
│   └── 🌅 Object A.jpg
├── 📁 Object B
│   ├── 📄 Object B.max
│   ├── 📄 Object B.obj
│   └── 🌅 Object A.jpg
├── 🌅 cover.jpg
└── 📄 library.json
```

`cover.jpg`

Justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, diam voluptua.

`library.json`

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.

```json
{
    "author":"Sanaa",
    "description":"A collection of people silhouettes in Revit, Illustrator, and Rhino file formats, curated by the architectural firm Sanaa for use in their designs and projects. These detailed silhouettes are easily accessible and can be incorporated into a variety of design and architectural projects.",
    "tags":[
        "Design",
        "Architecture"
    ]
}
```

### Object

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.

```
📁 Object
│   ├── 📄 Object.max
│   ├── 📄 Object.obj
│   └── 🌅 cover.jpg
```

## Cloud

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.

## Members

At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.

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

### Q: Is there a live demo available?
A: Yes, you can find a live demo of this project at [https://your-project-demo.com](https://your-project-demo.com).
