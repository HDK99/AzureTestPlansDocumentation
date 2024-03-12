## Create manual test cases
_Overview:_
- Manual test cases are essential for validating deliverables against user needs.
- These cases include detailed steps, encompassing shared steps and parameters for testing different data.
_Organization and Execution:_
- Organize test cases by adding them to test plans and suites.
- Assign testers to run the tests efficiently.
_Prerequisites:_
- Ensure project connectivity; create one if not available.
- Users must be added to a project.
- Basic access or higher is required for viewing test-related work items.
- Basic + Test Plans access or specific Visual Studio subscriptions are necessary for test plans, suites, and configurations.
- Various permissions are needed for adding, modifying, and managing test-related artifacts.
_Important Notes:_
- Test iterations are designed for data-driven scenarios, not workflow-driven ones.
- New users should review "Navigate Test Plans" for UI guidance.
- Uninstall the deprecated "Test manager for TFS 2017 and TFS 2018" extension if Basic access suffices for required functionalities.
## Create test cases

1. If you haven't already,[[Azure DevOps/Test Plans/Get Started/Create Test Plans and Test Suites|create a test plan and requirement-based test suites]].
2. Select a requirement-based test suite and select **New Test Case**.![[Pasted image 20240306174525.png]]
3. **Click or type here to add a step**.![[Pasted image 20240306174550.png]]
4. **Add** test steps, describing actions and expected results, **Attachments** can be included for clarity. **Repeat** until all test steps are added.
Explore further details in [[Azure DevOps/Test Plans/Get Started/Share Steps Between Test Cases|Share Steps]] and [[Azure DevOps/Test Plans/Get Started/Copy-Clone Test Plans, Suites, Cases|Copy or clone stories, issues and other work items]]
## Assign configurations to test cases
Specify configurations: operating systems, web browsers, and other variations for your tests.
-- Select the test suite > **More options** > **Assign configurations**, and in the dialog box, select your configurations
![[Pasted image 20240306175216.png]]

You can also assign configurations to individual test cases. Select the cases, **More options** > **Assign configuration**.

- Make your changes and then **Save**.

For more information, see [[Azure DevOps/Test Plans/Manual Tests/Test Different Configurations|Test Different Configurations]].

## Reorder test cases

![[Pasted image 20240310145903.png]]

## Add existing test cases to a test suite

![[Pasted image 20240310145950.png]]

![[Pasted image 20240310150019.png]]

## Use the Grid view to edit test cases

1. ![[Pasted image 20240310150046.png]]
2. ![[Pasted image 20240310150054.png]]
3. ![[Pasted image 20240310150124.png]]
4. ![[Pasted image 20240310150141.png]]

## Assign testers
~Testers need [Basic access](https://learn.microsoft.com/en-us/azure/devops/organizations/security/access-levels?view=azure-devops) to run tests from Azure Test Plans.


You can reassign test cases so that a different tester can run them. You can assign all the test cases in a test suite to **multiple** testers, which is **useful** for **acceptance testing**.
1. ![[Pasted image 20240310150330.png]]
2. ![[Pasted image 20240310150341.png]]

You can assign an individual test case to a tester.

1.![[Pasted image 20240310150554.png]]

## Manage test cases

You can open a test case to view it or edit it.
1.  In the **Define** tab, double-select the name of the test case.
2. ![[Pasted image 20240310194833.png]]

### Use tags for test cases
**Functionality*:
- Tagging allows categorization of test cases.
- Example: Tag tests related to signing in for easy rerun after fixing related bugs.
- Tags provide a filtering mechanism in the Test Plans web portal.

**Requirements*:
- Basic access or higher required.
- Project-level permission to create new tag definitions must be set to Allow.
- For adding and editing tags:
    - Can be done during test case editing.
    - Bulk editing available in Grid view.

**Enhancements*:
- Create suites based on queries using tags.

## Rename or remove test cases
![[Pasted image 20240310200710.png]]
And from there u can either delete or rename, but you will need the **Basic + Test Plans**.

