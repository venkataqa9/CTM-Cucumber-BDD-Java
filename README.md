# CTM-Cucumber-BDD-Java

# Prerequisites

First unzip the project.
- Download Apache Maven.
- Now download eclipse or intellij and double click on eclipse.exe and now it will ask to create
  workspace.
- Create a directory for project.
- Now you can create a new java project or if you already have an existing project
  unzip it and import it.
- In the next step we have to choose (Use an execution environment JRE 1.7 or 1.8)
- Add environment variables
  Java_Home C:\Program Files\java-jdk-path
  Maven_Home C:\apache-path
  Class_Path C:\Program Files\java\jre version\bin; C:\Program Files\java\jdk version\bin;

### Project Structure
bdd
├── src
|   ├──  main/               # main package
|   ├── factory/             # package
|       └──DriverHelper      # open broser and close browser
        └──Pages             # common method waitForVisibilityOfElement
    ├── pageObjects/         # package     
|   |   └── EnergyPage.java  # EnergyPage
|   |   └── EnergyQuote
        └── HomePage.java    # EnergyQuoteHomePage
|   |   └── LoginPage.java   # LoginPage
|   |   └── YourDetails.java # YourDetails
|   |   └── YourResults.java #   LoginPage 
    ├── utils/               # package
    |       └──Helpers       # method to get environment file

|   ├──  test/               # main package
      ├──java/      
          └── hooks.java     # Before and After annotations
|   |     └── runTest.java   # Runner class to run test
│   ├── resources            # package
|   |   ├── config/          # package
|   |   └── env.props        # browser and url poperties
                             # Scenarios for:
│   ├── features/            # Cucumber support files
|   |   └──quotes.feature    # Scenarios
├── screenshots/             # Folder for screenshots (Git ignored)
├── pom.xml                  # For storing all dependencies

# To run Tests:
Mvn clean test 
Or 
Right click on RunTest to run tests 

