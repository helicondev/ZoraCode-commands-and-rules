# Fix Error Command

A command to systematically analyze and resolve specific errors in the codebase.

## Usage
/fix-error [error-message]

## Template
Use the following systematic approach to analyze and resolve the error:

{{input}}

REQUIRED PROCESS:
1. First review ALL files involved in this error
2. Identify the exact root cause of the problem
3. Propose ONLY the minimal fix needed (do not refactor)
4. Verify your solution actually resolves the specific error
5. Briefly explain why this solution works

VALIDATION REQUIRED:
After implementing the fix, you MUST compile and run linter to confirm the error is actually resolved.

IMPORTANT: Only fix what's necessary to resolve the error, keep the rest of the code intact.