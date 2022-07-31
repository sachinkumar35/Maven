# Maven
Maven is a build automation tool used primarily for java projects. Maven uses <b>convention</b> over <b>configuration</b> which means developers are not required to create build process themselves. Maven provides sensible default behavior for projects. When a maven project is created, it creates default project structure and developer is only required to place files accordingly.

There are many problems that you may face during the project development which are discussed below : 

    1. Adding set of Jars in each project : In case of selenium projects , we need to add multiple jar files each project . 
    2. Dependencies and Versions : Ensuring that the jar files and the required dependencies are added to the project for developing , compiling and executing the same.

# Maven structure
POM in Maven stands for Project Object Model. It is fundamental Unit of Work in Maven. It is an XML file which resides in the base directory of the project as pom.xml. The POM contains information about the project and various configuration detail used by Maven to build the projects. 

POM also contains the goals and plugins. While executing a task or goal, Maven looks for the POM in the current directory. It reads the POM, gets the needed configuration information, then executes the goal.
