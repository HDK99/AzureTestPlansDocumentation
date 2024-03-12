When working in Azure DevOps, associating automated tests with test cases is a valuable practice. This enables you to run tests seamlessly as part of a test plan and ensures end-to-end traceability of requirements. Follow these steps to associate your automated tests with test cases.

## Prerequisites

- Visual Studio Enterprise or Professional 2017 or a later version.
- Access to Azure Test Plans.
- Knowledge of the identifier of the work item for the test case.

## Steps

### 1. Create a Test Project and Build Pipeline

- Create a test project containing your automated test. Ensure your test project supports the desired test types.
- Check in your test project into Azure DevOps.
- Create a build pipeline for your project, ensuring it includes the automated test. Note differences if using a XAML build.

### 2. Associate Your Test

1. Open your solution in Visual Studio Enterprise or Professional 2017 or a later version.
    
2. If you don't know the identifier of the work item for the test case:
    
    - Locate the test case in Azure Test Plans.
    - Or, query for the work item in the Work hub.
3. Once you know the identifier of the work item for the test case:
    
    - If using Visual Studio 2017 or a later version:
        - Open the **Test Explorer** window from the **Test | Windows** menu.
        - If your tests aren't displayed, build the solution.
        - In Test Explorer, select the test method to associate and choose **Associate to Test Case**.
        - In the dialog, type the test case identifier, choose **Add Association**, then **Save**.
    ![[Pasted image 20240312125602.png]]
    - The dialog lists test cases associated with the selected test method. You can't associate more than one test method with a test case, but a test method can be associated with multiple test cases.
4. If using Azure DevOps build and release services (not XAML build), you can run associated tests in build and release pipelines using the **Visual Studio Test** task. Running tests on-demand using Microsoft Test Manager is available only with XAML builds.
    
5. Note: Parameters in a test case aren't used by any automated test associated with it. Iterations using parameters are for manual tests only.

## Frequently Asked Questions (FAQs)

### Q: What types of tests are supported?

- Coded UI tests, Selenium tests, and unit tests using MSTest framework v1 can be associated with a test case.
- MSTest v2, NUnit, and xUnit tests can be associated with a test case (starting from Visual Studio 15.9 Preview 2).
- .NET core framework tests are supported (Visual Studio 15.9 Preview 2 or later).
- Tests using other frameworks (e.g., Chutzpah, Jest) cannot be associated.

### Q: What are the differences if I'm still using a XAML build?

- With XAML builds, you can run associated tests in a Build-Deploy-Test workflow using a Lab environment.
- Running tests using Microsoft Test Manager and a Lab environment is possible with XAML builds.

### Q: Can I configure work items to open in Visual Studio?

- Yes, change the Work Items | General setting from the Tools | Options menu in Visual Studio.
    ![[Pasted image 20240312125619.png]]

By following these steps and considering the FAQs, you can efficiently associate your automated tests with test cases in Azure DevOps. This not only streamlines your testing processes but also enhances traceability and quality assurance.