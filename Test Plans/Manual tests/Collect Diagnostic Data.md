## Prerequisites

1. Connect to your project. If not created, [create one](https://chat.openai.com/c/4a308997-d388-4111-a4e1-6608e2e70607#).
2. Ensure project or team membership.
3. Stakeholder access or higher for feedback.
4. `Edit work items in this node` permission required.
5. Permission to create tag definitions.

## Collecting Diagnostic Data

You can collect diagnostic data from both web and desktop apps during testing in Azure Test Plans.

### Web Apps

For web apps, use the web-based Microsoft Test Runner. It allows you to:

- Capture Screenshots
- Create Image Action Logs
- Record Screen

### Desktop Apps

For desktop apps, download and install the Test Runner desktop client. It provides on-demand collection of:

- Screen Captures
- Image Action Logs
- Screen Recordings

### Capture Your Screen

1. Open Test Runner and select the **Capture screenshot** icon.
2. Choose the app and drag to select the screen area. Annotate if necessary.
![[Pasted image 20240312124424.png]]
3. Save the screenshot.

### Capture Interactions as Image Action Log

1. Open or switch to Test Runner and choose **Capture user actions...** icon.
![[Pasted image 20240312124341.png]]
2. The Test Runner records all actions on the app's browser tab or desktop app.
3. Stop to finish capturing. The action log is added to test results.
![[Pasted image 20240312124409.png]]
### Record Your Screen

1. Open or switch to Test Runner and choose **Record screen** icon.
![[Pasted image 20240312124301.png]]
3. Choose the screen or app to start recording.
4. Stop recording when done. The recording is added to test results.

### View Diagnostic Data

- When creating a bug, all captured data is included.
- View and annotate diagnostic data before saving the bug.
![[Pasted image 20240312124149.png]]
### Play Video Recordings

- Use the appropriate extension to [play video recordings](https://learn.microsoft.com/en-us/azure/devops/test/reference-qa?view=azure-devops#recording-playback) created during testing.

### Advanced Diagnostic Data

- For advanced data (code coverage, IntelliTrace, Test Impact data), configure data collectors in Microsoft Test Manager and run tests using it.
## Conclusion

Efficiently collect and analyze diagnostic data during testing in Azure DevOps to ensure effective bug reporting and resolution.