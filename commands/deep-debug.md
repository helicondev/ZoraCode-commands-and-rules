# Deep Debug Command

A command to systematically deep debug the code.

## Usage
/deep-debug [file-path]

## Template
Use the following systematic approach to deep debug the code:

{{input}}

SYSTEMATIC DEBUG PROCESS:
1. ERROR ANALYSIS:
   - Parse error message components
   - Identify error type (compile-time, runtime, logical)
   - Trace error propagation path
   - Check error timestamp and frequency

2. ENVIRONMENT INVESTIGATION:
   - Verify dependencies and versions
   - Check configuration files
   - Analyze environment variables
   - Review recent changes (git log --oneline -10)

3. CODE FLOW TRACING:
   - Map execution path to error point
   - Identify all variables in scope at failure
   - Check function call stack
   - Analyze data transformations

4. ROOT CAUSE HYPOTHESIS:
   - Generate 3 possible causes ranked by likelihood
   - For each cause, specify validation method
   - Predict side effects of each potential fix

5. SOLUTION VALIDATION:
   - Provide fix with reasoning
   - List test cases to verify fix
   - Identify potential regressions
   - Suggest monitoring for future prevention

DELIVERABLE: Step-by-step debugging report with validated solution and prevention strategy.