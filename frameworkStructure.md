frameworkStructure.md

- Selenium - Web Automation
- Appium - Mobile Automation
- Rest Assured - API interactions
- TestNG - Unit Testing
- Extent Reports - Reporting
- Lombok - Removes Boilerplates
- Owner - Config File Management
- Maven - Build and Dependency Management Tool
- AssertJ - Fluent Assertions
- Webdrivermanager - Managing browser binaries
- Jackson - Serialisation and Deserialisation
- Awaitility - Async API calls
- NoException - Custom Exception Handlers to handle checked and unchecked exception
- Data Supplier - Customised Data Provider

Features : 

- Ability to run tests in local, remote, selenoid grid
- Run Android, IOS tests in local and remote (browser stack)
- Clean code principles 
- Reporting
- Unit tests
- Integration with Jenkins 
- Database Integration
- Code formatting
- Github Action Integration (Replacing Jenkins with Github action)
- Publishing results in Github pages.
- Dockerise the tests and push to external docker registry with Github actions.
- git-crypt secrets.
- How to write proper readme file, PR templates?


## Rule

- keep design principle
- maintainable


- Enum
    BrowserType
    RunMOde
    BrowserRemo
- config
    - factory
        for singleton 
    - converter
        take string in upper case and return the enu,
    - config interface


        Framework  

- Pages

Home page
    - component

        - Locators for Menu
        subMenu
        Logo

        click Menu
        Click sub Menu
        GetLogoSrti

    - Loca


    
    Base    
        loadAllFixuter
        inti

    driver
        get DriverData from Factory

            LocalDriverFactory 
                - chromeManager
                - FireFoxMan
            RemoteFactory
                - Selenoid
                    Manager
                - grif
                - b

    Test 