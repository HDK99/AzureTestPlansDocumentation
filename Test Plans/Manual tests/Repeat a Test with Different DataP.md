In manual testing, repeating a test with different data is crucial. Here's how you can achieve this in Azure DevOps:

### Prerequisites

1. Connect to a project. If needed, [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Be added to a project. To get added, [add users to a project or team](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
3. For viewing or adding test configurations, have Basic access or higher.

### Add Parameters to a Test Case

1. Create a parameter by typing a name preceded by "@" in the actions and expected results of your test steps.
    ![[Pasted image 20240312123520.png]]
2. Underneath the list of steps, add combinations of parameter values.

### Share Parameters Between Test Cases

1. In an open test case, select **Convert to shared parameters**.
    ![[Pasted image 20240312123525.png]]
2. After creating a shared parameter set, open another test case and add the shared parameter set.
    ![[Pasted image 20240312123530.png]]
3. Map the shared parameters to the local parameters if needed.
    ![[Pasted image 20240312123534.png]]
4. Add, edit, and rename shared parameter sets in the Parameters page.
    ![[Pasted image 20240312123537.png]]
5. Each shared parameter set is a work item; view or make changes in the Properties page.

### Run a Test Case with Parameters

1. Select a test case with parameters and start running it. The Test Runner shows the first row of parameter values.
    ![[Pasted image 20240312123544.png]]
2. When completing the steps, mark the test as passed or failed, and proceed to the next iteration with different parameter values.
    ![[Pasted image 20240312123550.png]]
3. Use the menu to navigate to other iterations.
    ![[Pasted image 20240312123554.png]]
4. Fix any incorrect parameter values without canceling the test by choosing Edit from step's shortcut menu.

### Review Test Results

1. To review test results, from the Execute tab, select a test point. Choose **View test results** from the context menu.
    ![[Pasted image 20240312123615.png]]
2. You can view the results in the Test Case Results dialog box.
![[Pasted image 20240312123629.png]]
### Speed Up Test Iterations by Using Record and Playback

To speed up iterations:

1. Create an action recording when you run the test with the first set of parameter values.
2. Play it back for other sets to reduce manual effort.

**Note**: Record and playback may not work with all applications; check [Supported configurations and platforms](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).

For more information, refer to related articles.