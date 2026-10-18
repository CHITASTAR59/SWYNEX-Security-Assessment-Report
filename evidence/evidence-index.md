# Evidence Index

## Purpose

This document tracks the evidence associated with the security assessment.

## Evidence Handling Rules

* Use only evidence obtained from an authorized environment.
* Use synthetic accounts and non-sensitive test data.
* Remove passwords, password hashes, session cookies, API keys, and tokens.
* Avoid collecting unrelated user information.
* Do not include confidential third-party screenshots without permission.
* Do not modify evidence in a way that misrepresents the observed result.

## Evidence Register

| Evidence ID | Finding | Description                           | Environment    | Status  |
| ----------- | ------- | ------------------------------------- | -------------- | ------- |
| E-01        | F-01    | Redirect validation test              | Not yet tested | Pending |
| E-02        | F-02    | Safe output-rendering test            | Not yet tested | Pending |
| E-03        | F-03    | CSRF validation test                  | Not yet tested | Pending |
| E-04        | F-04    | Cross-account authorization test      | Not yet tested | Pending |
| E-05        | F-05    | Cross-organization authorization test | Not yet tested | Pending |

## Evidence Requirements

For each completed test, record:

1. Test date.
2. Application name and version.
3. Authorized test environment.
4. Test objective.
5. Expected behavior.
6. Observed behavior.
7. Result.
8. Evidence filename.
9. Relevant limitations.

Do not mark pending evidence as collected or completed.
