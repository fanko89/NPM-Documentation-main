# What is NPM? What does it do? Why is it an important tool?
'Node Package Manager' is a tool that simplifies package management for Node.js developers. It provides a wide range of pre-built components, known as 'packages', which can be easily downloaded and managed using NPM. This allows developers to save time by reusing existing code, instead of having to make everything from scratch. With NPM, developers can easily find, download, and manage packages, along with their dependencies.
NPM is an important tool for Node.js developers, enabling them to easily reuse pre-built code packages, saving time and effort while building high-quality applications. Moreover, NPM fosters collaboration and knowledge-sharing among developers, pushes creativity and improving the overall quality of Node.js applications, ultimately benefiting the industry as a whole.

# What problems does NPM Slove?
NPM solves challenges for Node.js developers by providing a centralized registry of open-source packages, enabling easier management of external dependencies and promoting collaboration and sharing of code. NPM also helps to improve the quality of code by promoting the use of well-maintained, well-tested packages.

# Describe the 3 main parts of NPM.
- **Semantic versioning** (semver) to manage package versions and ensure compatibility between packages, dependencies, and projects.

 - **CLI** (command-line interface), which provides a way for developers to interact with the NPM registry and manage their packages.

- **Scripts** to automate common development tasks, such as testing, building, and deploying their code. These scripts are defined in the package.json file and can be executed using the NPM CLI.

# What is the package.json file?
 It is used to define a project's metadata and configuration, including its version, dependencies, and scripts.

# What is the scripts section of the package.json file? How do you use it? What are the default commands, and how do you use your own?
- The package.json file has a "scripts" section for custom commands to run with the npm run command. Scripts automate tasks like testing and deploying code. A key-value pair structure is used to define each script name and its associated command.
![script example](/pic/script.png)
 - To use a script, you need to add a key value-pair to the 'script' section of the 'package.json' file. Then in the commandline 'npm run (script name)'. If you were using the script exsmple above, you'd type in the command line 'npm run dev' to run 'vite dev'.
- The default commands are 'test', 'start', and 'install'.
- To use your own customs commands, you would need to define it in the scripts section of the 'package.json' fine.

# What are dependencies? What does this section define? What are dev dependencies? Why is it important to define dev dependencies vs dependencies?
- Dependencies are modules required for a 'node.js' project to function properly.
Semantic versioning ranges can also be defined in this section to control how dependencies are updated and ensure long-term stability. 

![Dev dependencies example](/pic/dev%20depend.png)
- Dev dependencies are packages or modules that are only required during the development and testing of a Node.js project, not during its production use. These dependencies are defined in the 'devDependencies' section of the package.json file, and can be installed using the 'npm install' command with the '--dev' or '-D' flags.

- Dependencies are required for the project to run unlike dev dependencies that are only needed for development. Separating these dependencies keeps the production environment efficient, and only providing necessary development tools. This ensures consistent build and testing across different environments because dev dependencies might not need to be installed in production.

# How do you install dependencies? Where do dependencies get installed?
Dependencies section of the 'package.json' file lists the external packages and modules that a 'Node.js' project needs to function properly. When a project is installed with 'npm install', all NPM's dependencies are automatically downloaded and installed to the 'node_modules' directory.

# When running scripts with NPM, where does NPM look (path) for the dependencies of those scripts?
When NPM runs scripts, it looks for the dependencies required to execute those scripts in the project's node_modules directory. This directory is created in the root of the project when the dependencies are installed using the npm install command.

# Name 3 NPM commands, and why they are important.

**Npm install** -  Installs all of the project's dependencies as defined in the package.json file.

**npm install (package)** - Installs a specific package or module as a dependency for the project.

**npm run (script)** - Runs a script defined in the package.json file's "scripts" section. This is useful for automating tasks such as testing, building, or deploying the project.

Using these commands is vital because they provide an organized and intuitive method of managing dependencies, creating new projects, executing scripts, and upgrading packages. This improves consistency and proper maintenance of the project, while also minimizing the risk of compatibility issues and errors.









