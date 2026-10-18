# Security Assessment Methodology

## 1. Preparation

Identify the assessment objective, permitted systems, testing boundaries, and documentation requirements.

No production testing should be conducted without appropriate authorization.

## 2. Information Review

Review supplied vulnerability descriptions and identify:

* Affected functionality.
* Suspected vulnerability category.
* Security boundary.
* Required attacker capabilities.
* Potential consequences.
* Missing evidence.
* Assumptions requiring validation.

## 3. Threat Modeling

For each finding, assess:

* The assets being protected.
* The trust boundary involved.
* The potential attacker's privileges.
* The required preconditions.
* The expected security control.
* The possible confidentiality, integrity, and availability impact.

## 4. Validation Planning

Define a controlled test using a locally deployed application or an explicitly authorized assessment environment.

Use synthetic accounts and non-sensitive data.

Establish the expected secure behavior before testing.

## 5. Evidence Collection

Record:

* A unique finding identifier.
* The test environment.
* The application version.
* The date of authorized testing.
* The expected result.
* The observed result.
* Relevant sanitized evidence.
* The remediation recommendation.

Do not collect unnecessary personal data, credentials, password hashes, session cookies, or authentication tokens.

## 6. Severity Assessment

Estimate severity based on:

* Exploitability.
* Required privileges.
* User interaction.
* Confidentiality impact.
* Integrity impact.
* Availability impact.
* Scope of affected resources.
* Business consequences.

Use a recognized scoring methodology when sufficient evidence is available.

## 7. Remediation Validation

Repeat the authorized test after the fix.

Confirm that the vulnerability is no longer reproducible and that legitimate functionality still works.

## 8. Reporting

Document each finding using a consistent structure:

1. Finding ID.
2. Title.
3. Summary.
4. Affected component.
5. Verification status.
6. Technical analysis.
7. Impact.
8. Severity.
9. Remediation.
10. Regression-test criteria.

## 9. Reporting Limitations

A vulnerability should not be reported as confirmed unless sufficient evidence establishes the behavior.

Historical descriptions, unverified claims, and hypothetical scenarios must be labeled accurately.
