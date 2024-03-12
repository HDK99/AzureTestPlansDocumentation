## Supported Clients and Run Options:

- **Clients:**
    
    - Microsoft Test Runner for Web Browser
    - Test Runner Client for Desktop Applications
    - Microsoft Test Manager 2017 Client
    - Microsoft Test Manager 2015 or Earlier Client
- **Run Options:**
    
    - Manual tests using Web Browser-based runner.
    - Manual tests using Test Runner client.
    - Automated tests using release stage.
    - Manual tests using Microsoft Test Manager 2017 client.
    - Manual tests using Microsoft Test Manager 2015 or earlier client.

## Prerequisites: 

- Connect to a project.
- Be added to a project.
- Basic access or higher is required to view or run manual or automated tests.

##Work with the TCM Command-line Tool:

- Install Visual Studio 2017 Professional or an earlier version.
- Access TCM from the command prompt using specific directories.
- Use parameters like `/collection`, `/teamproject`, and `/login` as needed.

## Run Tests for Web Apps:
1. Open the web portal, navigate to Test Plans > Test plans.
    
2. Create manual tests if not done already.
    
3. Select Mine or All, or use Filter by title to find your test plan, then go to the Execute tab.
    ![[Pasted image 20240312122405.png]]
4. Choose one or more tests or all tests from a suite, then select **Run for web application.**
    ![[Pasted image 20240312122414.png]]
5. Microsoft Test Runner opens in a new browser; start the app you want to test.
    
6. Mark each test step as passed or failed based on expected results.
    ![[Pasted image 20240312122358.png]]
7. If a test step fails, enter a comment and create or add to a bug.
    

## Create or Add to a Bug:

1. When a step fails, enter a comment and select Create bug.
    ![[Pasted image 20240312122329.png]]
2. In the New bug dialog, enter a bug name, and the steps/comments are automatically added.
    ![[Pasted image 20240312122333.png]]
3. You can assign, comment, or link to other issues. Save & Close when done.
    
4. Instead of creating a bug, you can update an existing bug by selecting Add to existing bug.
    

**Note:** Ensure correct team settings at the Area and Iteration levels for proper bug creation.

