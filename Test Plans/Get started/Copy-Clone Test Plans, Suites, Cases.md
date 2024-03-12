
## Overview
Several tools support copy, clone, or import operations for Azure DevOps test items, facilitating efficient test management. Test cases, suites, and plans are integral parts, each serving specific functions.

## Supported Tools
Depending on your Azure DevOps version, you can utilize various clients and tools for copying, cloning, or importing test plans, test suites, and test cases. These tools include the Web portal, TCM command-line tool, and REST API.

### Key Tools
- **Web portal:** Copy, import, and bulk export/import test plans, suites, and cases.
- **TCM CLI:** Clone and import automated test cases via command line.
- **REST API:** Provides cloning functionality for test plans and test suites.

## Prerequisites
Ensure you have the necessary permissions and access levels, such as Basic, Basic + Test Plans, or specific Visual Studio subscriptions. Familiarize yourself with the TCM command-line tool for advanced operations.

## Copying Test Plans
Create new test plans for each project milestone, easily copying or cloning existing plans. Choose reference or duplication based on your branching strategy.

## Importing or Cloning Test Suites
Efficiently reuse test suites for new sprints by importing or cloning. Shared steps and parameters are also cloned, streamlining the process.

## Copying Test Cases
Copy individual or multiple test cases within or across projects. Maintain flexibility with options to include existing links and attachments.

## Bulk Import/Export
Perform bulk import or export of test cases using CSV files. Customize the export by selecting specific test cases or entire suites.

## Importing Automated Test Cases (TCM)
Utilize the TCM command-line tool to import automated test cases, specifying parameters like storage path, priority, and categories.
![[Pasted image 20240312121541.png]]
## Limitations and Tips
Be aware of limitations, such as the Design state requirement for test case state columns, and ensure the user performing import/export has the necessary permissions.

Explore additional REST APIs for copying and cloning test plans and suites.

For more detailed information, refer to the [Azure DevOps documentation.](https://learn.microsoft.com/en-us/azure/devops/test/copy-clone-test-items?view=azure-devops&tabs=tcm-cli#list-test-plans-or-test-suites)
