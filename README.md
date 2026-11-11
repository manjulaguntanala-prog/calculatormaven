# Calculator Maven Project

A beginner-friendly Java Maven project with basic calculator operations and JUnit 5 tests.

## Requirements
- JDK 11 or later
- Apache Maven 3.8 or later

## Run from Command Prompt (Windows)
Open Command Prompt in the folder containing `pom.xml`, then run:

```bat
mvn clean test
mvn package
```

The generated JAR will be in `target/`.

## Import into Eclipse
1. Extract the ZIP.
2. Open Eclipse.
3. Choose **File > Import**.
4. Select **Maven > Existing Maven Projects**.
5. Browse to the extracted `calculator-maven-project` folder.
6. Select the project and click **Finish**.

## Use with Jenkins
1. Make sure Jenkins has the **Maven Integration** plugin if you want to create a Maven project job.
2. Configure Maven under **Manage Jenkins > Tools** and give the installation the name `Maven`.
3. Configure a JDK installation named `JDK`, or edit the `tools` names in the Jenkinsfile to match your configured names.
4. Create a Pipeline job and connect it to your Git repository, or use the Jenkinsfile in this project.
5. This Jenkinsfile uses Windows `bat` commands. For a Linux agent, replace `bat` with `sh`.
