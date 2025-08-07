# Code Review Command

A command to systematically analyze the code.

## Usage
/code-review [file-path]

## Template
Use the following systematic approach to analyze the code:

{{input}}

MANDATORY ANALYSIS PROCESS:
1. SECURITY SCAN: Check for SQL injection, XSS, CSRF, authentication bypasses, data leaks
2. BUG DETECTION: Identify null pointer exceptions, race conditions, memory leaks, logic errors
3. PERFORMANCE AUDIT: Find O(n²) algorithms, unnecessary loops, inefficient queries, memory waste
4. CODE QUALITY: Check naming conventions, function length (>50 lines), cyclomatic complexity (>10)
5. BEST PRACTICES: Verify error handling, input validation, logging, separation of concerns

OUTPUT FORMAT:
- CRITICAL ISSUES (security/bugs): [List with line numbers and severity]
- PERFORMANCE PROBLEMS: [Specific bottlenecks with impact estimation]
- CODE SMELLS: [Maintainability issues with refactor suggestions]
- POSITIVE ASPECTS: [What's well implemented]

VALIDATION: After providing feedback, explain HOW to verify each suggested fix works.