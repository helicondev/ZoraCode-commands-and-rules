# Fix Error Command

A command to systematically analyze and resolve specific errors in the codebase.

## Usage
/fix-error [error-message]

## Template
Use the following systematic approach to analyze and resolve the error:

{{input}}

Apply the Error Resolution Guidelines defined in the project rules:

1. Initial Diagnosis
   - Read the complete stack trace
   - Identify the specific file and line number
   - Determine the error type (syntax, runtime, logical, dependency)

2. Contextual Investigation
   - Examine related code within a 10-15 line radius
   - Verify imports and dependencies
   - Review relevant configuration files (package.json, tsconfig, etc.)

3. Resolution Strategy
   - For TypeScript errors: Check types and interfaces
   - For dependency errors: Verify installation and versions
   - For runtime errors: Add validations and handle edge cases
   - For syntax errors: Correct immediately

4. Implementation and Validation
   - Apply the specific fix
   - Run relevant tests
   - Verify no regressions are introduced
   - Document the change if necessary

5. Future Prevention
   - Suggest improvements to prevent similar errors
   - Add tests if they don't exist
   - Propose refactoring if needed

Provide a detailed explanation of the error and the steps to fix it.