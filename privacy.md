# Baseline Guard — Privacy Policy

[Documentation](documentation.html) · [Support](support.html) · **Privacy Policy** · [End User Terms](terms.html)

**Effective date: August 25, 2026**

Baseline Guard ("the App") is a Jira Cloud application built on the Atlassian Forge platform. It evaluates Jira project evidence and produces evidence-backed project assessments and reporting for Executive, Client, and Internal audiences.

This Privacy Policy explains what information Baseline Guard accesses and processes and how that information is handled.

**Brian Levy, doing business as Levy Automations** ("we," "us," or "our") operates Baseline Guard.

For privacy or support questions, contact **help@levyautomations.com**.

## 1. What Baseline Guard Does

Baseline Guard reads selected information from a Jira Cloud project when an authorized user generates an assessment.

The App uses available Jira evidence to evaluate project status, evidence confidence, risks, commitments, decisions, proposed actions, and evidence limitations.

Baseline Guard is designed to avoid presenting unsupported assessments when the available Jira evidence is insufficient.

## 2. Information Baseline Guard Accesses

When an authorized user generates an assessment, Baseline Guard accesses selected information from the Jira project chosen by that user.

Using Jira's `read:jira-work` permission, this may include:

- Jira issue keys
- Issue summaries
- Issue status and status category
- Issue type
- Priority
- Created, updated, resolution, and due dates
- Labels
- Parent issue information
- Sprint information
- Assignee information associated with relevant issues

The information accessed depends on the project, reporting period, available Jira evidence, and selected reporting audience.

Baseline Guard does not request the `read:jira-user` scope and does not access the customer's Jira user directory through that scope.

Baseline Guard does not fetch Jira comments.

Baseline Guard respects the Jira permissions of the user generating the assessment.

## 3. Information Baseline Guard Stores

**Baseline Guard does not persist Jira issue content or generated assessments as a separate customer data store.**

Assessments are generated on demand from Jira evidence available at the time of generation.

Baseline Guard does not intentionally store Jira issue summaries, comments, descriptions, generated assessment content, or other Jira issue content in application storage.

Local interactions or edits to a generated report are page-local and are not persisted by Baseline Guard.

Baseline Guard does not intentionally log Jira issue content.

## 4. Data Retention

Because Baseline Guard does not persist Jira issue content or generated assessments as a separate customer data store, it does not maintain a retention period for generated assessments.

A newly generated assessment evaluates the Jira evidence available at the time it is generated.

Operational platform information may be processed by Atlassian as necessary to provide and operate the Forge platform, subject to Atlassian's applicable policies and platform practices.

## 5. Why We Process Information

Baseline Guard processes Jira information only as necessary to provide the App's functionality.

This includes:

- Reading authorized Jira project evidence
- Generating project assessments
- Displaying assessment results
- Evaluating evidence confidence and limitations
- Producing audience-appropriate reporting
- Validating evidence references
- Enforcing App licensing
- Diagnosing application failures without intentionally logging Jira issue content

We do not use customer Jira data for advertising, marketing, or user profiling.

We do not sell customer Jira data or personal information.

## 6. AI and Large Language Model Processing

Baseline Guard uses AI-assisted generation through Atlassian's native Forge LLM capability.

Relevant Jira context may be processed using models made available through Atlassian Forge to assist with structured analysis and reporting.

Baseline Guard applies validation and governance controls to generated output and validates evidence references against Jira issues available to the assessment.

Baseline Guard distinguishes facts from interpretations where appropriate and identifies recommendations as recommendations rather than established facts.

When required evidence is insufficient, Baseline Guard may return a **NOT ASSESSABLE** result rather than manufacture a supported project assessment.

Baseline Guard does not require customers to provide external AI API keys.

Baseline Guard does not intentionally transmit customer Jira issue data to an independently operated external AI service controlled by Levy Automations.

## 7. Data Sharing and Service Providers

Baseline Guard is built and hosted using Atlassian Forge.

The App does not operate an independently hosted application backend for processing customer Jira issue data.

Atlassian processes information as part of providing the Forge infrastructure and services on which Baseline Guard operates.

We do not sell customer information or share customer Jira data with advertisers or data brokers.

## 8. Hosting

Baseline Guard is built and hosted on the Atlassian Forge platform.

Application processing occurs using Atlassian-hosted Forge infrastructure.

Baseline Guard is designed without external network egress for customer Jira issue data.

Customers should consult Atlassian's current documentation for information regarding Forge infrastructure, hosting, and applicable data residency capabilities.

## 9. Security and Access Controls

Baseline Guard is designed according to least-privilege principles.

Baseline Guard:

- Uses read-only Jira access for assessment and reporting
- Does not require Jira write permissions for assessment generation
- Respects the permissions of the current Jira user
- Does not fetch Jira comments
- Does not intentionally persist Jira issue content or generated assessments
- Does not intentionally log Jira issue content
- Validates evidence references used in generated assessments
- Separates evidence-supported facts from interpretations and recommendations where appropriate

Baseline Guard does not claim an independent security certification.

## 10. Personal Information

Baseline Guard may process personal information contained in Jira issue data when necessary to generate an assessment, such as an assignee display name associated with an issue.

Baseline Guard does not request access to the customer's Jira user directory through the `read:jira-user` scope.

Baseline Guard does not intentionally persist personal information contained in Jira issue content as a separate customer data store.

## 11. Your Privacy Requests

The organization operating your Jira Cloud site controls the underlying Jira information available to Baseline Guard.

Users with questions concerning information stored in Jira should generally contact their organization's Jira administrator.

For questions concerning Baseline Guard's data practices, contact **help@levyautomations.com**.

We will review and respond to reasonable requests as appropriate.

## 12. Children's Privacy

Baseline Guard is business software intended for use by organizations.

It is not directed to children under the age of 16, and we do not knowingly collect personal information from children through the App.

## 13. Changes to This Privacy Policy

We may update this Privacy Policy to reflect changes to Baseline Guard, Atlassian's platform, legal requirements, or our data practices.

When material changes are made, we will update the effective date at the top of this policy and, where appropriate, provide notice through the Atlassian Marketplace or another reasonable channel.

## 14. Contact

**Baseline Guard**

Operated by Brian Levy, doing business as Levy Automations

**Levy Automations**  
421 W Riverside Ave #381  
Spokane, WA 99201  
United States

Email: **help@levyautomations.com**

For questions about this Privacy Policy or Baseline Guard's data practices, contact us at the email address above.
