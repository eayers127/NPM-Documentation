1. What is NPM? What does it do? Why is it an important tool?
NPM used to stand for Node Package Manager. It is now the package manager for just about every langauge, so it is now not only the Node package manager.
There used to be several package managers, but now NPM does all of the work for us.
It is used for installing packages - libraries or frameworks. Packages live in the NPM Registry and are downloaded to a file called "Node Modules".
NPM is a registry, which is a fancy way of saying that it is a database/storage area.

2. What problems does NPM solve?
NPM finds and downloads files from different sources.

3. Describe the 3 main parts of NPM?
NPM is a command line tool, a registry, and a website.
Command line tool: tool used to install and update packages.
Registry: Data storage area
Website: Where libraries and frameworks are stored and then shared by developers. 

4. What is the package.json file?
The package.json file holds metadata. It is required for almost all projects. In a .json file the key value pairs must be in "" ,and .json files cannot contain comments.
The package.json file also defines functional attributes of the project.

5. What is the scripts section of the package.json file? How do you use it? What are the default commands, and how do you use your own?
The scripts section is where the user can create/add scripts that can be entered in the terminal or command line to run different actions.
The user adds a new script in the "scripts" {} be typing the name of the script in "" followed by a : and then quotes with a description of what the script completes.
I have learned more about this through my internship. We have a local site for our documentation and I was trying to get this site up and running. Someone showed me the package.json file with all sorts of scripts that I could run in order to make changes to the documentation.
The script I was looking for was labeled "start". So I ran "npm run start" in the terminal and I got the local site up and running.
There was also a script named "all" which fires the rest of the scripts in a particular order. This command was helpful when I was pushing a change the code.
This image shows an example of the scripts located in a package.json file. Each of these scripts can be ran in the terminal.
![image](https://user-images.githubusercontent.com/71342594/216794650-becb5492-16b3-49a2-9f18-7aed4755b543.png)


6. What are dependencies? What does this section define? What are dev dependencies? Why is it important to define dev dependencies vs dependencies?
A dependency is when one package depends on another package in order to function. This can result in a dependency tree which is one package depends on another package that depends on another package and so on.
Dev dependencies are the things in the package.json file that are required for a project to run on the local host. Examples of dev dependencies are Webpack and Babel
Dev dependencies are needed during the development of the project, so they are important to define in order to be able to create the project. Once in production, these dependencies are no longer needed.

7. How do you install dependencies? Where do dependencies get installed?
NPM install should add all of the necessary dependencies
Most dependencies can be found in the "node-modules" file
Additional dependencies can be added.


8. When running scripts with NPM, where does NPM look (path) for the dependences of those scripts?
Scripts are run from the root of the package folder

9. Name 3 NPM commands, and why they are important.
 I use npm run local everyday at my job. That gets our local component library open in a new tab so that I can view the components on the current branch.
 NPM audit can be used to run a security audit. Cyber security is getting more and more important and relevant, so this command is an easy way to try to stay on top of keeping your code secure.
 While researching more about npm, I read about npm ci which installs a project with a clean slate. This is useful for builds that will be repeated and automated, like a testing environment.
