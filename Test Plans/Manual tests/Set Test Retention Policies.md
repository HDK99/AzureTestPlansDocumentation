Running tests, particularly automated ones, generates substantial data that can impact system performance. To maintain system responsiveness and efficiency, it's crucial to implement policies for clearing unnecessary test results. This article guides you through setting up retention policies for both manual and automated test results in Azure DevOps.

## Prerequisites

- To manage project-level test-related policies, you need to be a member of the **Project Administrators** group.
- For managing build pipeline object-level test retention policies, ensure you have the **Edit build pipeline** permissions set to Allow.

## Set Retention Period for Manual Test Results

1. Sign in to your project at https://dev.azure.com/{Your_Organization}/{Your_Project}.
2. Select **Project settings**.
3. Navigate to **Test > Retention** page.
4. Choose a limit for how long you want to retain manual test data.
    ![[Pasted image 20240312125421.png]]

This ensures that manual test results are retained for a specified period, allowing you sufficient time for analysis.

## Set Retention Policy for Automated Test Results Associated with Builds

Azure DevOps, by default, retains automated test results related to builds only as long as you keep those builds. To retain test results even after builds are deleted:

1. Sign in to your project at (`https://dev.azure.com/{Your_Organization}/{Your_Project}`).
2. Find and edit your **build pipeline**.
    ![[Pasted image 20240312125440.png]]
3. Open the **Retention** page and modify default policies or add new ones.
    ![[Pasted image 20240312125443.png]]
    If you use Git, you can specify retention based on branches, allowing you to keep test results in specific branches while deleting builds in others.
    

## Set Retention Policy for Automated Test Results Not Associated with Builds

Clearing up automated test results that are not linked to builds or from deleted builds is essential. For instance, results published from external test systems. Follow these steps:

1. Set retention limits at the project level, as mentioned in the **Set Retention Period for Test Results** section.
2. Adjust retention limits for automated test results not associated with builds.

By configuring these retention policies, you ensure that your testing data is efficiently managed, preventing unnecessary clutter and maintaining optimal system performance.

## Conclusion

Implementing test retention policies in Azure DevOps is a crucial aspect of efficient test data management. By specifying how long to retain manual and automated test results, you can strike a balance between keeping valuable data for analysis and preventing an overload of unnecessary information.