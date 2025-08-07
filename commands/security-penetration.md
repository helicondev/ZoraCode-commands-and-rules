# Security Penetration Command

A command to systematically analyze the security of the codebase.

## Usage
/security-penetration [file-path]

## Template
Use the following systematic approach to analyze the security of the code:

{{input}}

COMPREHENSIVE SECURITY AUDIT:
1. AUTHENTICATION & AUTHORIZATION:
   - Test for privilege escalation vectors
   - Check session management and token security
   - Verify password policies and hashing methods
   - Analyze role-based access control implementation

2. INPUT VALIDATION TESTING:
   - Test all input points with malicious payloads
   - Check for SQL injection in all query contexts
   - Test XSS in stored, reflected, and DOM contexts
   - Verify file upload restrictions and validation

3. DATA PROTECTION ANALYSIS:
   - Check encryption at rest and in transit
   - Verify sensitive data handling (PII, credentials)
   - Analyze logging practices for data leakage
   - Test backup and recovery security

4. INFRASTRUCTURE SECURITY:
   - Check dependency vulnerabilities (npm audit, etc.)
   - Analyze configuration security
   - Test for information disclosure
   - Verify error handling doesn't leak information

5. BUSINESS LOGIC TESTING:
   - Test workflow bypass scenarios
   - Check for race conditions in critical operations
   - Verify transaction integrity
   - Test edge cases in business rules

DELIVERABLE: 
- CRITICAL VULNERABILITIES: [Immediate fixes required]
- SECURITY RECOMMENDATIONS: [Ranked by risk level]
- EXPLOITATION SCENARIOS: [How attackers could exploit found issues]
- REMEDIATION GUIDE: [Specific code changes with examples]
- COMPLIANCE CHECK: [OWASP Top 10, GDPR, etc. alignment]