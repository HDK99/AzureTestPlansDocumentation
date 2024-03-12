## Prerequisites

1. Connect to your project. If not created, [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Ensure you are added to a project or team.
3. Stakeholder access or higher is required for feedback.
4. Have the `Edit work items in this node` permission set to Allow.
5. Permission to create tag definitions.

## Introduction

User Acceptance Testing (UAT) is crucial for ensuring that software meets business requirements and maintains high quality. This guide provides insights into assigning and managing UAT in Azure DevOps.

## Prerequisites

- Connect to your project. [Create a new project](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#) if required.
- Ensure project or team membership.
- Stakeholder access or higher for feedback.
- `Edit work items in this node` permission for bugs and other work item types.
- Permission to create tag definitions.

## Assign and Invite Testers

1. Navigate to **Test plans** and open your desired test plan.
2. Choose a test suite and select **More options** or right-click to access the context menu. Then, click on **Assign testers to run all tests**.

3. In the **Search users** box, enter the name of testers. Multiple testers can be selected.
    ![[Pasted image 20240312124025.png]]
    > Note: Users must be members of the Project Valid Users group. User groups cannot be selected.
4. To notify testers, select **Send email**. Enter a subject and note, then click **Ok**.
    ![[Pasted image 20240312124044.png]]
5. For individual test case assignment, go to the **Execute** tab, select a test case, and choose **More options**. Then, click **Assign tester** and use the search option to find a tester.
    ![[Pasted image 20240312124049.png]]

## Track Results

- Focus on individual test runs or leverage chart views for effective result tracking.
- The dashboard provides a comprehensive overview, supporting various testing types.

> If the expected data is missing, ensure that the necessary columns are added to the **Tests** view.

## Conclusion

User Acceptance Testing is streamlined in Azure DevOps, allowing efficient tester assignment and result tracking. Utilize these features to ensure software meets business requirements seamlessly.