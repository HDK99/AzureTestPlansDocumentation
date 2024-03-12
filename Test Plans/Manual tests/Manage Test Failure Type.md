# Add, run, and update inline tests in Azure Boards and Azure DevOps
## Prerequisites

1. Connect to your project, or [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Ensure you are added to a team or project.
3. Have Basic access or higher for work items and board features.
4. Have `View work items in this node` and `Edit work items in this node` permissions set to Allow.

## Open Your Kanban Board

- Navigate to your project in a web browser.
- Select **Work**, then **Boards**, and choose your team's board.
![[Pasted image 20240312123827.png]]
## Add Inline Tests

1. Open the context menu of a backlog item to add inline test cases.
    ![[Pasted image 20240312123832.png]]
2. Tests are added similarly to test cases in a test suite, automatically creating a test plan and suite for the user story.

3. If adding many tests, keep entering titles and select Enter.

## Run Inline Tests

1. Run a test by selecting the Run icon from the actions menu.
    ![[Pasted image 20240312123921.png]]
2. Microsoft Test Runner opens in a new browser instance.

## Update Test Status

- Update the test status from the actions menu to track test results.
    ![[Pasted image 20240312123925.png]]

## Expand or Collapse Inline Tests

- Inline tests are initially collapsed. Select the inline test summary to expand/collapse the list.

## Copy or Reparent a Test

- To reparent, drag and drop the test onto a different user story.
    ![[Pasted image 20240312123937.png]]
- To create a copy, press the CTRL key, then drag and drop the test onto another user story's card.

## Related Articles

- Utilize inline tests for lightweight traceability and manual test management.
- [Create manual tests](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#) for more details on defining tests.

## Test Status in Kanban Board

- Track test outcomes easily with the integrated test status in the Kanban board.
- **Note**: For complex scenarios with multiple configurations, consider using Test Manager for comprehensive testing progress tracking.