![[Pasted image 20240312122832.png]]
Your users may interact with your app on various configurations like different operating systems, web browsers, and more. To ensure thorough testing, you can set up and run tests in different configurations. Follow these steps:

### Prerequisites

1. Connect to a project. If none exists, [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Be added to a project. To get added, [add users to a project or team](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
3. For viewing or adding test configurations, have Basic access or higher.
4. For adding test configurations, ensure the project-level Manage test configurations permission is set to Allow (By default, granted to Contributors and Project Administrators groups). For details, see [Manual test access and permissions](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).

### Work with the TCM Command-Line Tool

Make sure you have the following in place:

- Installed Visual Studio 2017 Professional or an earlier version.
- Access TCM from the command prompt in the specified directories.

Use the TCM command-line tool with parameters such as /collection, /teamproject, and /login as needed.

### View Configurations and Variables

#### Browser

1. Navigate to Test Plans > Configurations from the left navigation area in the Test Plans web portal.
2. You'll see all test configurations and variables for your test plans.
3. Select a configuration or variable to view detailed information.

#### TCM CLI

Execute a command to view a list of test configurations and configuration variables.

### Create Configurations and Variables

1. Open the **Configurations** page in the **Test Plans** web portal.
2. Select the + icon, then New configuration variable.
3. Type a name (e.g., Browser), add values, and save.
4. Create additional variables (e.g., **Operating system**) with their values.
5. Select the + icon and **New test configuration.**
6. Type a name, add the created variables with values, and ensure "**Assign to new test plans**" is checked.
7. Save your new test configuration.

### Assign Configurations to Test Plans and Suites

- To assign configurations to a test suite, select a plan, go to Test Suites, choose a suite, and assign configurations.
![[Pasted image 20240312123115.png]]
- For individual test cases, select one or more, open the context menu, and choose Assign configuration.

### Run Tests with Each Configuration

1. Set up a testing platform for a specific configuration (e.g., Google Chrome on Windows 10).
2. Select and run a test with this configuration.
3. The status bar will display a reminder of the configuration as you run the test.
![[Pasted image 20240312123154.png]]
### Track Test Results for Each Configuration

1. Open the Charts page for your test suite.
2. Select New, then New test result chart.
3. Choose a chart type, select Group by > Configuration, and click OK.
![[Pasted image 20240312123214.png]]
4. A chart is created to track tests based on configurations. Pin it to your dashboard if needed.
![[Pasted image 20240312123230.png]]
### Note

If a test case appears in multiple test suites, you can set different configurations for each suite. The same test case can have different configuration settings in different test suites and test plans.