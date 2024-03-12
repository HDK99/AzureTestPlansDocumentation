## Overview
Azure Test Plans users can efficiently manage test cases through bulk import or export using CSV or Excel formats. The import operation supports both creating new test cases in a designated suite and updating existing ones by providing the test case ID. The export operation allows exporting test cases into CSV or XLSX formats.

### Key Actions
1. **Export Test Cases:**
   - Navigate to Test Plans > Test plans.
   - Choose the desired test plan and suite.
   - Optionally select Column options for customization.
   - Export all or a subset of test cases to CSV or XLSX.
![[Pasted image 20240312121843.png]]

2. **Import Test Cases:**
   - Select the target test plan and suite.![[Pasted image 20240312121828.png]]
   - Choose the file to import (CSV or XLSX).
   - Confirm the import, and handle overwriting of existing elements if applicable.

3. **Update Existing Test Cases:**
   - Create a column view with desired fields.
   - Export test cases to CSV or XLSX.
   - Make necessary edits without altering ID and Work Item Type.
   - Save the file and import it back to the test suite.
![[Pasted image 20240312121811.png]]
4. **Import Automated Test Cases (TCM):**
   - Use the TCM command-line tool with parameters like storage path, priority, and category.
   - Specify the suite ID for synchronization within the test plan.

## Important Notes
- Native web-portal functionality supports additional operations like copy, clone, and update test cases.
- Ensure adherence to limitations, such as maintaining ID and Work Item Type during updates.
- Explore REST APIs for advanced copying and cloning of test plans and suites.
