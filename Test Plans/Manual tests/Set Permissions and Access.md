Azure DevOps provides robust testing features that require specific permissions and access levels to ensure effective test management. This article outlines the prerequisites and steps to grant access, manage test plans and suites, and set permissions for creating and deleting test artifacts.

## Prerequisites

To exercise the full features of Azure Test Plans, users must have one of the following subscriptions:

- Enterprise
- Test Professional
- MSDN Platforms

In addition, users need Basic + Test Plans access level to utilize Azure Test Plans fully.

## Access and Permissions

Access and permissions are managed at different levels: Object-level, Area path level, Project-level, and Organization or collection-level.

### Object-level, Area path level

1. **Edit work items in this node:** Add or edit test-specific work items.
2. **Manage test plans:** Modify test plan properties.
3. **Manage test suites:** Create and delete test suites, modify test suite hierarchy.

### Project-level

1. **Manage test configurations:** Add or edit test configurations and configuration variables.
2. **Manage test environments:** Add or edit test plan settings.
3. **Create test runs:** Run manual tests.
4. **Delete and restore work items:** Delete test-specific work items.
5. **Delete test runs:** Delete test results.
6. **Move work items out of this project:** Move work items to another project.
7. **Permanently delete work items:** Permanently delete test-specific work items.

### Organization or collection-level

1. **Manage test controllers:** Associated with a deprecated feature for TFS 2018 and later versions.

## Prerequisites for Managing Permissions

- To manage access levels or organization-level permissions, be a member of the Project Collection Administrators security group.
- To manage project or object-level test-related permissions, be a member of the Project Administrators security group.

## Granting Access to Manual Testing Features

Users must have Basic + Test Plans access level for full access to the Test feature set. Users with Basic access and permissions to permanently delete work items can only delete orphaned test cases.

## Managing Test Plans and Test Suites under an Area Path

1. Open the Security page for area paths.
2. Choose the user or group to grant permissions.
3. Set permissions for **Manage test plans** and **Manage test suites** to Allow.

## Setting Permissions to Create and Delete Test Artifacts

Deleting test artifacts involves permanent deletion with specific considerations:

- Only supports permanent deletion of test artifacts, and they cannot be restored.
- Deletes all associated child items such as child test suites, test points, testers, and test results history.
- Must be a member of the Project Administrators group or have the **Delete test artifacts** permission set to Allow.
- Access level must be set to Basic + Test Plans or Visual Studio Enterprise.

## Conclusion

Effectively managing permissions and access levels is crucial for leveraging Azure DevOps Test Plans. This ensures secure and streamlined test management, allowing teams to take full advantage of the testing features provided by the platform.