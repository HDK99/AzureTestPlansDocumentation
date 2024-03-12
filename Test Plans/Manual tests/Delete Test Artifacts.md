## Prerequisites

1. Connect to your project. If not created, [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Membership in the Project Administrators group or project-level `Delete test runs` permission set to Allow is required to delete test runs.
3. To delete test plans and test suites, you need to be a member of the Project Administrators group or have the Area Path node-level `Manage test plans` or `Manage test suites` permission set to Allow.
4. Access level set to Basic + Test Plans or Visual Studio Enterprise.
5. Users with Basic access and permissions can only delete orphaned test cases, i.e., those not linked to any test plans or test suites.
6. Permanently deleting a test artifact also deletes all associated test artifacts like test results.
7. Bulk deletion of test artifacts is not supported.

## Work Item Types Supporting Test Experience

- Test Cases
- Test Plans
- Test Suites
- Shared Steps
- Shared Parameters
![[Pasted image 20240306163107.png]]

## Deleting a Test Case, Test Suite, or Test Plan

1. Open the test case, test suite, or test plan from the web portal.
2. Choose the **Permanently delete** option from the actions menu. (Bulk deletion is not supported from a query results page.)
![[Pasted image 20240312124813.png]]
3. Confirm the deletion.

4. To delete a test plan directly from Test Plans, open Test Plans, choose **More Actions** for the plan, and select **Delete**.

5. For shared steps and shared parameters, manually remove all references before deleting.
![[Pasted image 20240312124828.png]]
## Conclusion

Deleting test artifacts in Azure Boards requires careful consideration as it permanently removes associated data. Ensure proper permissions and follow the steps outlined for efficient and secure deletion.