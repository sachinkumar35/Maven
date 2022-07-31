# Maven
Maven is a build automation tool used primarily for java projects. Maven uses <b>convention</b> over <b>configuration</b> which means developers are not required to create build process themselves. Maven provides sensible default behavior for projects. When a maven project is created, it creates default project structure and developer is only required to place files accordingly.

There are many problems that you may face during the project development which are discussed below : 

    1. Adding set of Jars in each project : In case of selenium projects , we need to add multiple jar files each project . 
    2. Dependencies and Versions : Ensuring that the jar files and the required dependencies are added to the project for developing , compiling and executing the same.

# Maven structure
POM in Maven stands for Project Object Model. It is fundamental Unit of Work in Maven. It is an XML file which resides in the base directory of the project as pom.xml. The POM contains information about the project and various configuration detail used by Maven to build the projects. 

POM also contains the goals and plugins. While executing a task or goal, Maven looks for the POM in the current directory. It reads the POM, gets the needed configuration information, then executes the goal.

A maven repository is a directory of packaged JAR file with pom.xml file. Maven searches for dependencies in the repositories. 
There are 3 types of maven repository: 
    
    1. Local Repository 
    2. Central Repository 
    3. Remote Repository 

Maven searches for the dependencies in the following order. 

        LOCAL REPOSITORY ---------> CENTRAL REPOSITORY -----------> REMOTE REPOSITORY

Note: If dependency is not found in these repositories, maven stops processing and throws an error.

# Maven Local Repository 
Maven local repository is located in your local system. It is created by the maven when you run any maven command.

By default, maven local repository is <b>%USER_HOME%\.m2</b> directory. 

    For example: C:\Users\<<Username>>\.m2. 
    
# Maven Central Repository 

Maven central repository is located on the web. It has been created by the apache maven community itself. 

Please access the <b>central repository</b>. The central repository contains a lot of common libraries that can be viewed by using the search page. 

# Maven Remote Repository 

Maven remote repository is located on the web. Some libraries can be missing from the central repository and may be required to be downloaded from the individual repositories by the firm. 

    Eg: JBoss library file needs to be downloaded from the JBoss nexus repository.

# Installation and configuration of Maven project

The key points about Maven Installation and configuration: 

    1. The plugin is being installed from the Eclipse Marketplace. 
    2. An update URL is used for installation. 
    3. CCD Permission/Open internet is required to perform the installation through Eclipse Marketplace .
    4. Installation success can be verified by checking for the availability of Maven preference under the option Window - > Preferences.
    5. To configure maven in the machine, the <b>MAVEN HOME</b> environment variable has to be set.  
    6. The variable should contain the path to the maven bin installable. eg: If the installable is in the ath: C:\maven\apache-maven-3.3.9, the environment variable should contain the value: C:\maven\apache-maven-3.3.9\bin 
    7. The configuration can be verified by opening command prompt and typing mvn -version. 
    8. The settings.xml file provided by the tools group should be placed inside C:\Users\<<Username>>\.m2. Please download the settings.xml file. 
    9. The settings.xml file should also be kept inside the conf folder inside the maven bin installable.
