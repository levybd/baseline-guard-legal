# Baseline Guard — Privacy Policy

**Effective date: August 21, 2026**

Baseline Guard ("the App") is a Jira Cloud app built on the Atlassian Forge platform that turns a Jira project's activity into concise, decision-ready status briefs for Executive, Client, and Internal audiences, with statements traceable to the Jira issues behind them.

This Privacy Policy explains what information the App accesses, stores, and processes and why. It applies to customers who install and use Baseline Guard through the Atlassian Marketplace.

**Brian Levy, doing business as Levy Automations** ("we," "us," or "our") operates Baseline Guard.

For privacy or support questions, contact **help@levyautomations.com**.

## 1. What Baseline Guard Does

Baseline Guard reads selected information from a customer's Jira Cloud instance and uses that information to generate a project status brief for the project, reporting period, and audience selected by the user.

Depending on the available Jira evidence, a brief may contain information such as project status, trend, confidence, risks, decisions, immediate actions, and supporting evidence.

Baseline Guard is designed to refuse to produce unsupported assessments when the Jira evidence does not satisfy its required baseline conditions.

## 2. Information Baseline Guard Accesses

When an authorized user generates a brief, Baseline Guard accesses selected information from the Jira project chosen by that user.

Using Atlassian's `read:jira-work` permission scope, this may include:

- Jira issue keys;
- Issue summaries;
- Issue status and status category;
- Issue type;
- Priority;
- Created, updated, resolution, and due dates;
- Labels;
- Parent issue information;
- Sprint information; and
- Display names of Jira assignees associated with relevant issues.

Baseline Guard also accesses the requesting user's Atlassian Account ID. This allows the App to associate a generation request with the user who submitted it and to enforce access controls when results are retrieved.

Baseline Guard does not read Jira comments, issue descriptions, all Jira issue fields, or the customer's Jira user directory.

For Executive and Client briefs, assignee names and certain internal details are excluded from information sent for AI-assisted generation.

## 3. Information Baseline Guard Stores

Baseline Guard stores limited information using Atlassian-hosted Forge storage associated with the customer's App installation.

Stored information may include:

- The Atlassian Account ID of the user who submitted a generation request;
- The selected Jira project, reporting period, and audience;
- Generation job status and error information;
- Generated brief content;
- Structured report information such as status, trend, confidence, claims, and related analytics; and
- Information necessary to determine whether the App installation has an active license.

Generated briefs may contain information derived from Jira, including issue summaries and assignee or owner display names where applicable to the selected audience.

Baseline Guard does not store Jira issue descriptions or Jira comment content.

## 4. Retention and Deletion

Baseline Guard uses limited retention periods for generation jobs and results.

In-progress generation jobs are retained for up to **1 hour**.

Completed generation results are retained for up to **7 days**, after which they expire from the App's active Forge storage.

Data stored through Atlassian Forge is associated with the customer's App installation. Following uninstall, Atlassian may retain Forge-hosted App data for a limited recovery period in accordance with Atlassian's Forge storage lifecycle.

Customers may request deletion of information controlled by Baseline Guard by contacting **help@levyautomations.com**.

## 5. Why We Process Information

Baseline Guard processes Jira and user information only as necessary to provide and operate the App.

This includes:

- Generating project briefs;
- Displaying generated results;
- Associating generation jobs with the requesting user;
- Enforcing authorization;
- Verifying that users continue to have appropriate project access;
- Enforcing App licensing;
- Operating generation jobs; and
- Diagnosing generation failures through limited operational information.

We do not use customer Jira data for advertising, marketing, or user profiling.

We do not sell customer Jira data or personal information.

## 6. AI and Large Language Model Processing

Baseline Guard uses AI-assisted generation through Atlassian's Forge platform.

Relevant Jira context may be processed by models made available through Atlassian's Forge platform to draft portions of a project brief.

Baseline Guard applies deterministic validation and governance rules to the generated output. These controls are designed so that status, trend, confidence, and other governed assessments must be supported by the underlying Jira evidence.

When mandatory baseline requirements are not satisfied, Baseline Guard may refuse to generate an assessed project status rather than send the request through the AI-generation path.

For Executive and Client briefs, assignee names and certain internal details are excluded from the information provided for AI-assisted generation.

Baseline Guard does not maintain its own external AI API keys or send Jira information from the App to an independently operated external AI service.

## 7. Data Sharing and Service Providers

Baseline Guard does not operate its own external application servers and does not intentionally transmit customer Jira data to external services operated by Levy Automations.

The App uses Atlassian's Forge platform for application hosting, storage, asynchronous processing, and supported AI capabilities.

Accordingly, Atlassian processes information as part of providing the infrastructure and services on which Baseline Guard operates.

We do not sell customer information or share it with advertisers or data brokers.

## 8. Hosting and Data Residency

Baseline Guard is built and hosted on the Atlassian Forge platform.

The App's application processing and Forge storage are Atlassian-hosted, and Baseline Guard does not require an independently operated external backend server.

Baseline Guard is designed without external network egress for customer Jira data.

Data stored using Forge hosted storage is subject to Atlassian's applicable Forge hosting and data residency capabilities.

Customers should consult Atlassian's current documentation for information about supported Forge data residency locations and controls.

## 9. Security and Access Controls

Baseline Guard is designed according to least-privilege principles.

The App requests the Jira and Forge permissions required to perform its functions, including `read:jira-work` and `storage:app`.

Baseline Guard includes authorization controls intended to:

- Associate generated results with the requesting user;
- Verify Jira project access;
- Prevent unauthorized retrieval of generated results;
- Prevent generation by installations without an active license; and
- Prevent unsupported project assessments when required Jira evidence is unavailable.

Customer information stored by the App remains within Atlassian-hosted Forge infrastructure.

Baseline Guard does not claim an independent security certification.

The App has been designed to satisfy the technical eligibility requirements for Atlassian's Runs on Atlassian program.

## 10. Your Privacy Requests

The organization that operates your Jira Cloud site controls the underlying Jira information available to Baseline Guard.

Users with questions about Jira information should generally contact their organization's Jira administrator.

For questions or requests concerning information stored specifically by Baseline Guard, including requests concerning access, correction, or deletion, contact:

**help@levyautomations.com**

We will review and respond to reasonable requests as appropriate.

## 11. Children's Privacy

Baseline Guard is a business software product intended for use by organizations.

It is not directed to children under the age of 16, and we do not knowingly collect personal information from children through the App.

## 12. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes to Baseline Guard, Atlassian's platform, legal requirements, or our data practices.

When we make material changes, we will update the effective date at the top of this policy and, where appropriate, provide notice through the Atlassian Marketplace or another reasonable channel.

## 13. Contact

**Baseline Guard for Jira**  
Operated by **Brian Levy, doing business as Levy Automations**

**Levy Automations**  
421 W Riverside Ave #381  
Spokane, WA 99201  
United States

Email: **help@levyautomations.com**

For questions about this Privacy Policy, Baseline Guard's data practices, or privacy-related requests, contact us at the email address above.
