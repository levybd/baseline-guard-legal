# Baseline Guard for Jira — Security Policy

[Documentation](documentation.html) · [Support](support.html) · [Privacy Policy](privacy.html) · [End User Terms](terms.html) · **Security**

**Effective date: September 2, 2026**

This Security Policy describes how Baseline Guard for Jira is secured and how security concerns are handled. Baseline Guard is operated by **Brian Levy, a sole proprietor, operating as Levy Automations**.

## 1. Scope and security boundary

Baseline Guard is a Jira Cloud app built and hosted on Atlassian Forge. Its application functions, asynchronous processing, queue, key-value storage, and native Forge large-language-model capability run on Atlassian-hosted Forge services. Baseline Guard does not operate an independently hosted application backend and is designed without external network egress for customer Jira issue data.

Atlassian operates and secures the Forge platform and Jira Cloud infrastructure under Atlassian's own policies and practices. Levy Automations is responsible for the Baseline Guard application code, its requested permissions, application-level authorization controls, dependency maintenance, and response to reported security issues. Atlassian's platform controls are not represented as independent Levy Automations certifications or controls.

## 2. Access and authorization

Baseline Guard requests read-only Jira work access for assessments and does not request Jira write access or the Jira user-directory scope. Jira project access is checked in the context of the requesting user before a job is accepted and again before a stored result is returned.

Generation jobs are bound to the Atlassian account identifier of the requesting user. A stored result is returned only when the current user matches that binding, remains entitled to use the app, and still has access to the Jira project. These application checks supplement, and do not replace, Jira's own permission controls.

## 3. Data handling and storage

Jira information needed for an assessment is processed within Atlassian Forge. Baseline Guard does not fetch Jira comments and does not intentionally log Jira issue content.

Baseline Guard stores generation-job records in Atlassian Forge Key-Value Store (KVS) so asynchronous work can complete and the requesting user can retrieve the result. Active **QUEUED** and **RUNNING** records receive a one-hour time-to-live when written. Terminal records, including completed, failed, and non-assessable results, receive a seven-day time-to-live when written. The applicable time-to-live is applied again when a record is updated, and records may be deleted earlier through the app's personal-data reporting process. Details are provided in the [Privacy Policy](privacy.html).

## 4. General application security controls

Baseline Guard uses the following application-level controls:

- least-privilege Forge scopes, including read-only Jira work access;
- user-context Jira project checks before job submission and result retrieval;
- requestor binding for stored generation jobs and results;
- entitlement checks before paid-app operations and stored-result retrieval;
- schema and evidence-reference validation for report contracts;
- state-based Forge KVS expiration for generation-job records;
- scheduled personal-data reporting and deletion for accounts Atlassian identifies as closed; and
- no external network egress declaration for customer Jira issue data.

No software system can be guaranteed to be completely secure. Baseline Guard does not claim an independent security certification.

## 5. Dependency and vulnerability management

Levy Automations reviews security reports and relevant security or maintenance updates affecting Baseline Guard's application dependencies and Forge integration. Confirmed vulnerabilities are assessed in the context of the app's architecture, permissions, reachable functionality, and potential customer impact.

When a change is warranted, Levy Automations develops and validates a proportionate correction and releases it through the applicable Atlassian Forge and Marketplace process. Priority and timing depend on severity, exploitability, customer impact, and the availability and safety of a correction. No fixed remediation time or service-level commitment is promised by this policy.

## 6. Security issue and incident handling

Privately reported or otherwise identified security concerns are reviewed to determine whether they affect Baseline Guard, customer information processed by the app, or the app's Forge configuration. Response may include preserving relevant non-sensitive operational information, containing affected application behavior, preparing and validating a correction, coordinating with Atlassian when the Forge or Jira platform is involved, and communicating appropriate information to affected customers.

If a confirmed incident materially affects customer information or use of Baseline Guard, Levy Automations will provide notice when reasonably appropriate and consistent with applicable legal obligations, the information available, and any necessary coordination with Atlassian or other authorities. This policy does not promise continuous monitoring, a guaranteed notification deadline, or a contractual incident-response service level.

## 7. Responsible vulnerability reporting

Report suspected vulnerabilities privately to **help@levyautomations.com**. Include a concise description, affected functionality, reproduction steps, and potential impact, while excluding credentials, access tokens, unnecessary personal data, and confidential Jira content.

**Do not disclose vulnerabilities, exploit details, secrets, credentials, personal data, or confidential Jira content through the public GitHub Issues support portal.** Public issues are visible to everyone. Account, privacy, and security matters must use the private email route above.

Levy Automations will acknowledge and evaluate good-faith reports through the normal support process. This is not a bug-bounty program and does not establish payment eligibility or guaranteed response or remediation times.

## 8. Customer responsibilities

Customers are responsible for securing their Atlassian accounts, managing Jira users and project permissions, protecting credentials, limiting sensitive Jira content to authorized users, and reviewing Baseline Guard outputs before relying on them for significant decisions.

## 9. Policy updates and contact

This policy may be updated to reflect material changes to Baseline Guard, its security practices, legal requirements, or the Atlassian platform. The effective date above identifies the current version.

Security questions and private vulnerability reports: **help@levyautomations.com**

**Operator and mailing address**

Brian Levy, operating as Levy Automations<br>
421 W Riverside Ave #381<br>
Spokane, WA 99201<br>
United States
