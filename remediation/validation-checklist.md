# Security Remediation Validation Checklist

## General

* [ ] The test environment is explicitly authorized.
* [ ] Synthetic accounts are used.
* [ ] The application version is documented.
* [ ] Expected secure behavior is defined.
* [ ] Evidence collection follows the approved scope.
* [ ] Sensitive data is excluded from evidence.

## F-01: XSS / Redirect Handling

* [ ] Approved redirects work.
* [ ] Unapproved destinations are rejected.
* [ ] Unexpected URL schemes are rejected.
* [ ] Untrusted input is rendered safely.
* [ ] Equivalent localized workflows are reviewed.

## F-02: Password-Reset XSS

* [ ] User-controlled values are safely rendered.
* [ ] Password values are not unnecessarily reflected.
* [ ] Reset tokens are handled securely.
* [ ] Error pages safely render unexpected input.
* [ ] Normal reset functionality works.

## F-03: GraphQL CSRF

* [ ] State-changing operations enforce the intended request policy.
* [ ] Unsupported HTTP methods are rejected.
* [ ] Required CSRF checks are enforced.
* [ ] Cross-origin requests cannot perform unauthorized mutations.
* [ ] Legitimate authenticated operations work.

## F-04: Account Deletion

* [ ] Authentication is required.
* [ ] Account ownership is verified server-side.
* [ ] Cross-account deletion is rejected.
* [ ] Invalid sessions are rejected.
* [ ] Unauthorized attempts do not change account state.
* [ ] Sensitive authentication data is not logged.

## F-05: Organization Member Deletion

* [ ] The target organization is resolved server-side.
* [ ] The target member's organization relationship is verified.
* [ ] The requesting user's permissions are checked.
* [ ] Cross-organization deletion is rejected.
* [ ] Unauthorized attempts leave membership records unchanged.
* [ ] Administrative events are logged appropriately.

## Final Approval

* [ ] Evidence has been reviewed.
* [ ] Regression tests have passed.
* [ ] Remaining limitations are documented.
* [ ] The finding status reflects the observed result.
* [ ] The responsible reviewer has approved closure.
