Part 1: Creating a SpringBoot Application
Introduction:
Spring boot is an open source most popular Java Framework which provides flexibility, efficiency, security, ease to the Java Developers.

Things you need:
IDE
JDK 1.8 or later
Gradle or Maven

This project is currently using IntelliJ CE as IDE, Java 11 JDK file and maven as dependency tool.

Step by step process to create a simple SpringBoot Application:

1. Open the IntelliJ IDE. Click on File -> New -> Project

2. Select the project type as Spring Initializer

3. Now, it's time to give it a name. 
Group:  specifies the id of the project group. It is actually a set of directories path in which the artifact resides.
Artifact: specifies the id of the project. It is actually the project name.
Type: Could be maven or gradle. Let's start with a maven project.
Version: Could update the version of the project. It is by default set to 0.0.1-SNAPSHOP
Group and Artifact automatically sets the package.

4. On the bottom right, you will see an option to import maven changes. Click on Enable Auto-import. This will install all the maven dependencies.

5. Open HelloWorldApplication.java file. This is the main spring boot application file from where the execution starts.

6. On the top right corner, You will see an option called HelloWorldApplication where different configurations related to the project could be added. Beside it, there is an arrow symbol used to run this application and a bug symbol used to debug the application.

7. Click on the arrow symbol beside the HelloworldApplication on the top right. The application starts running which could be seen in the logs as below

Note: 
An other way to create a springboot project is by going to https://start.spring.io/ website.

Give the group, artifact and other details and also select the dependencies that you  would need for that project and click on Generate.

This generates a zip file of spring boot project into your system.

Unzip the file and now, go to intelliJ and go to File -> New -> Project From Existing Resources -> Select the unzipped file -> Next -> Import from External Model -> Maven -> Next -> Select the Root Directory (Where you want your project to be) -> Next -> Next -> Select JDK 11 -> Give the project name and click on Finish. 

Now, follow the steps from step 4. 

Part 2: Pushing the Changes to Github

Step 1: Go to your Github account. You will see a screen similar like below:

Step 2: Click on New on top left. Give name to the repository. I prefer this to match with your local repository. Let's give it as helloworld.

Step 3: Do not, initialize the repository with readme file.  Click on Create repository

Step 4: This creates a repository for the project

Step 5: It's time to push the local repository changes to Github.
Open any terminal. I would usually prefer the intelliJ terminal which is in the bottom of the IDE. Go to the location where you have the project.

Step 6: Initialize the project by git init command

Step 7: Now, link the Github repository to Git. Copy the URL that you see in your github repository

Step 8: Now, goto the terminal and type git remote add origin <url> 

Step 9: It creates all red marks in the java files.

Step 10: If this is the first time creating the git project and pushing them to Github, I would suggest to follow the steps in https://beginnersword.blogspot.com/2020/07/getting-started-with-git-and-github.html
from step 2.

Note: For below terminology, look at the above link
If not, add files to index by git add * -> to add all the files

Next, commit the code to head by git commit -m "any message"

Next, push the changes to Github by git push origin master

Give your Github credentials to push the changes. Username is your gmail id that you gave for the Github account.
