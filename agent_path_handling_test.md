# Agent Path Handling Test Procedure

## Purpose
This document describes the process for testing the file manager's path handling and user experience in a Cursor Windows environment. Our process centers around starting a fresh chat session, processing a prompt, and providing structured feedback.

## Test Prompt
```
You are running in a Cursor Windows environment.

Please use the `read_multiple_files` tool to read the following three files (use any absolute path style you think is valid for Windows):

- C:/Dev/mcp/test1.txt
- C:/Dev/mcp/test2.txt
- C:/Dev/mcp/test3.txt

Report back with:
1. The exact paths you used in your tool call.
2. Whether the tool was able to read each file, and if not, the error message for each.
3. Any feedback on the experience or confusion about path formats.
```

## Testing Process
1. **Start a fresh chat session** with the agent.
2. **Paste the test prompt** above into the session.
3. **Observe the agent's tool call and response.**
4. **Collect feedback** from the agent, focusing on:
   - Path formats accepted and used
   - Success or failure for each file
   - Any confusion or errors encountered
5. **Document the results** for review and future improvements.

## Notes
- This process ensures that each test is unbiased by prior context and reflects the default agent experience.
- The test is designed to confirm that the file manager robustly handles all common Windows path formats and provides a smooth user experience.
