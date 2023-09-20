# Managing Packages with NPM
npm (Node Package Manager), is a command line tool to install, create, and share packages of JavaScript code written for Node.js. There are many open source packages available on npm, so before starting a project, take some time to explore so you don't end up recreating the wheel for things like working with dates or fetching data from an API.

In this course, you'll learn the basics of using npm, including how to work with the package.json and how to manage your installed dependencies.

***

## How to Use package.json, the Core of Any Node.js Project or npm Package
When you are done, make sure a working demo of your project is hosted somewhere public. Then submit the URL to it in the Solution Link field.

The package.json file is the center of any Node.js project or npm package. It stores information about your project, similar to how the head section of an HTML document describes the content of a webpage. It consists of a single JSON object where information is stored in key-value pairs. There are only two required fields; name and version, but it’s good practice to provide additional information about your project that could be useful to future users or maintainers.

If you look at the file tree of your project, you will find the package.json file on the top level of the tree. This is the file that you will be improving in the next couple of challenges.

One of the most common pieces of information in this file is the author field. It specifies who created the project, and can consist of a string or an object with contact or other details. An object is recommended for bigger projects, but a simple string like the following example will do for this project.

***

## Add a Description to Your package.json
The next part of a good package.json file is the description field; where a short, but informative description about your project belongs.

If some day you plan to publish a package to npm, this is the string that should sell your idea to the user when they decide whether to install your package or not. However, that’s not the only use case for the description, it’s a great way to summarize what a project does. It’s just as important in any Node.js project to help other developers, future maintainers or even your future self understand the project quickly.

Regardless of what you plan for your project, a description is definitely recommended. Here's an example:

"description": "A project that does something awesome",

***

## Add Keywords to Your package.json
The keywords field is where you can describe your project using related keywords. Here's an example:

"keywords": [ "descriptive", "related", "words" ],
As you can see, this field is structured as an array of double-quoted strings.

***


## Add a Version to Your package.json
A version is one of the required fields of your package.json file. This field describes the current version of your project. Here's an example:

"version": "1.2.0",

***

## Expand Your Project with External Packages from npm
One of the biggest reasons to use a package manager, is their powerful dependency management. Instead of manually having to make sure that you get all dependencies whenever you set up a project on a new computer, npm automatically installs everything for you. But how can npm know exactly what your project needs? Meet the dependencies section of your package.json file.

In this section, packages your project requires are stored using the following format:

"dependencies": {
  "package-name": "version",
  "express": "4.14.0"
}
