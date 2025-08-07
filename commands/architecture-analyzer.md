# Architecture Analyzer Command

A command to systematically analyze the architecture of the codebase.

## Usage
/architecture-analyzer [file-path]

## Template
Use the following systematic approach to analyze the architecture of the code:

{{input}}

COMPREHENSIVE EVALUATION:
1. CURRENT STATE ASSESSMENT:
   - Map existing components and their responsibilities
   - Identify coupling levels between modules
   - Analyze data flow and dependency directions
   - Measure complexity metrics (cyclomatic, cognitive)

2. SCALABILITY ANALYSIS:
   - Identify bottlenecks at 10x, 100x current load
   - Analyze database query patterns and N+1 problems
   - Check caching strategies and invalidation logic
   - Review async/sync processing boundaries

3. MAINTAINABILITY REVIEW:
   - Evaluate code organization and module boundaries
   - Check abstraction levels and interface design
   - Analyze configuration management approach
   - Review testing strategy coverage

4. TECHNICAL DEBT AUDIT:
   - Identify shortcuts that will cause future problems
   - List deprecated dependencies and migration needs
   - Find duplicated logic and inconsistent patterns
   - Analyze documentation gaps

5. IMPROVEMENT ROADMAP:
   - Prioritize changes by impact/effort matrix
   - Provide specific refactoring steps with order
   - Suggest incremental implementation strategy
   - Include rollback plans for each change

OUTPUT: Detailed analysis document with actionable recommendations, timeline estimates, and risk assessments.