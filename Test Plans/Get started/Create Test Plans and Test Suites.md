## Work Items in Your Test Experience**

When managing multiple versions of your product, you can efficiently share and reuse test cases across development cycles. Initially, you create test cases for a specific product version. Subsequently, these test cases are incorporated into test plans for each development cycle or release. Optionally, you can organize them into separate test suites for better management.

After creating a test plan, you [[Azure DevOps/Test Plans/Manual Tests/Test Different Configurations|assign test configurations]] and [[Azure DevOps/Test Plans/Get Started/Create Test Cases|Testers]] to cover the required test matrix. Testers execute the tests until the product meets exit criteria. For subsequent development cycles, you can create new test plans and reuse the same test cases, ensuring a consistent testing approach.

Notably, any updates made to a shared test case automatically propagate to all associated test plans and test suites. For future product versions, the option to reuse existing test cases exists, but for more control over changes, copying or cloning test cases to create a new baseline is recommended. This approach avoids impacting previous test plans, providing a clearer versioning system.
## Create a test plan
Before you create a test plan, [define your backlog of requirements](https://learn.microsoft.com/en-us/azure/devops/boards/backlogs/create-your-backlog?view=azure-devops).
1. Sign in to your Azure DevOps project and select **Test Plans** > **Test Plans**.
![[Pasted image 20240306172522.png]]
2. Select **+ New Test Plan**.
![[Pasted image 20240306172638.png]]
3. Enter a name, verify that the area path and iteration are set correctly, and then select **Create**.
![[Pasted image 20240306172721.png]]
## Rename a test plan
![[Pasted image 20240306172740.png]]
## Delete a test plan

1. Select **Test Plans**.
2. Next to the test plan name, select **More Actions** > **Delete**.
3. The **Permanently delete test artifacts** dialog box explains exactly what gets deleted. Enter the test plan ID to confirm that you want to delete, and then select **Permanently delete**.
![[Pasted image 20240306172856.png]]
## Add a requirement-based test suite

 1. To add a suite to a test plan, select **More options** for the test suite, and then select **New Suite** > **Requirement based suite**.![[Pasted image 20240306173225.png]]
use requirement-based suites to group your test cases together. That way, you can track the testing status of a backlog item. Each test case that you add to a requirement-based test suite is automatically linked to the backlog item.
2. Add clauses to filter work items by iteration path and run the query to view matching backlog items.![[Pasted image 20240306173339.png]]
3. Select desired backlog items and **create suites**, automatically linking test cases to each selected backlog item.![[Pasted image 20240306173412.png]]
## Test Suite Management Overview

1. **Creation and Organization:**
    ![[Pasted image 20240306173618.png]]
    - Create static test suites to act as folders for grouping various test suites.
    - Utilize drag-and-drop functionality to arrange test suites and tests within a static test plan.
    2. **Tracking Changes:**
    - Access the work item for a test plan or test suite to view detailed change history.
    - Monitor specific actions in the **Test Suite** Audit field, including additions and removals of test cases.
3. **Exporting Test Plans and Cases:**
    ![[Pasted image 20240306173747.png]]
    - Export test plans, test suites, and test cases to CSV format for external use.
    - Adjust the report's test case fields by customizing column selection in the list view of the test suite.

**Note:**

- Ensure not to exceed 75 Test Suites in a single export operation, as the email system supports up to 1MB of data.

## Find a test case in a test plan

You can use filter

![[Pasted image 20240306173914.png]]

