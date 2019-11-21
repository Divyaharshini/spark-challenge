<h1>Check for VS Code Extensions</h1>
1. VS Code Extension: Maven for Java

2. VS Code Extension: Java Extension Pack
<h1>Instructions 1 - Start New Maven Project</h1>
Create a new project using Maven.

There should be a folder on your laptop where you keep your git projects. Go to this folder, e.g. 44517.
Open this parent folder in VS Code.
Click the VS Code Extensions icon. Verify you have the two required extensions. If not, install them.
Click the VS Code Explorer icon. From the menu, select:
View / Command Palette / Maven: Create Maven Project / archetype-quickstart-jdk8 / most recent version.
When the folder window opens, click your parent folder up at the top, click "Select Destination Folder".
<h1>Instructions 2 - Interactive Mode</h1>
groupId: edu.nwmissouri.yourname
artifactId: spark-challenge
version: HIT ENTER
package: HIT ENTER
Y: HIT ENTER
You will now have a spark-challenge project folder. Exit VS Code.

<h1>Instructions 3 - Code the project</h1>
Change directory into your new spark-challenge folder. Right-click and open your spark-challenge folder in VS Code.

Add a basic README.md. Use it to store your notes and commands.

When VS Code asks: "A build file was modified. Do you want to synchronize the Java classpath/configuration?" Answer "Always" to allow VS Code to generate these artifacts automatically.

<h1>Instructions 4 - Add to POM.xml</h1>
Copy the POM.xml from this repo to yours. Use CTRL-F to search for "isl" for "Intelligent Systems Lab". Change each occurance to match yourname in your groupId instead.
<h1> Clean, Compile, Create fat jar files.</h1>
mvn clean,

mvn compile,

mvn assembly:single
<h1>Execute :</h1>
java -cp target/spark-challenge-1.0.0-jar-with-dependencies.jar edu.nwmissouri.bheemireddy.App "data.txt"
