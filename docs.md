# Baseline Guard — Documentation

[Customer Documentation](documentation.html) · [Support](support.html) · [Privacy Policy](privacy.html) · [End User Terms](terms.html) · [Security](security.html)

## Overview

**Baseline Guard turns Jira evidence into clear, defensible project assessments and decision-ready reporting.**

Instead of relying on subjective status updates or manually reconstructing project health from Jira, Baseline Guard evaluates available Jira evidence to help teams understand:

- What is the current project status?
- What evidence supports that assessment?
- What requires attention?
- What evidence is missing?
- What actions should happen next?
- How confident should stakeholders be in the assessment?

Baseline Guard is built for project leaders, delivery teams, PMOs, consultants, and organizations that need project reporting they can explain and defend.

---

## Getting Started

After installing Baseline Guard, open **Baseline Guard** from the Apps section of Jira.

To generate an assessment:

1. Select a Jira project.
2. Choose a reporting period.
3. Select an audience: **Executive, Client, or Internal**.
4. Select **Generate**.

Baseline Guard evaluates Jira information available to the current user and produces an evidence-backed project assessment.

Baseline Guard is read-only. Generating an assessment does not modify Jira issues or project data.

---

## Understanding Your Assessment

Baseline Guard evaluates available Jira evidence rather than simply repeating Jira status fields.

An assessment can return one of three outcomes:

- **ON TRACK** — available evidence supports the current delivery position.
- **AT RISK** — available evidence indicates meaningful delivery exposure requiring attention.
- **NOT ASSESSABLE** — Jira does not contain sufficient evidence to support a defensible assessment.

### Why NOT ASSESSABLE Matters

NOT ASSESSABLE is an intentional safeguard.

Baseline Guard does not manufacture confidence when the underlying Jira evidence is incomplete.

When available evidence cannot support a defensible assessment, Baseline Guard identifies the deficiency so the team can understand what is missing and address it.

A missing answer is more useful than a confident answer unsupported by evidence.

---

## Evidence Confidence

A project assessment is only as reliable as the evidence supporting it.

Baseline Guard communicates evidence confidence to help users distinguish between a strongly supported assessment and one based on limited Jira information.

Where evidence is incomplete, Baseline Guard surfaces that limitation rather than silently filling the gap with assumptions.

This allows stakeholders to understand both the project assessment and the strength of the evidence behind it.

---

## Evidence and Traceability

Evidence is central to Baseline Guard.

Important conclusions are tied to the Jira information supporting them so users can understand why an assessment was reached.

Baseline Guard distinguishes between:

- **FACT** — information directly supported by available Jira evidence.
- **INTERPRETATION** — bounded analysis based on available Jira evidence.

This distinction helps stakeholders understand what Jira establishes directly and what represents evidence-based analysis.

Where source issues are presented, users can return to the underlying Jira issue for additional context.

Baseline Guard is designed to prevent unsupported Jira issues from being presented as evidence for a conclusion.

---

## Reporting Periods

Baseline Guard supports several reporting periods for common project and delivery cadences.

Available reporting periods include:

- **Last 7 days**
- **Last 14 days**
- **Last 30 days**
- **Current Sprint**
- **Custom Range**

The assessment is generated using Jira evidence available for the selected project and reporting period.

---

## Executive Reporting

Executive reporting is designed to answer the questions leadership needs answered without requiring executives to interpret Jira workflow details.

Executive reporting emphasizes:

- Overall project status
- Evidence confidence
- Significant delivery exposure
- Commitments requiring attention
- Executive attention items
- Material risks
- Decisions requiring leadership attention
- Proposed next actions
- Known evidence limitations

Routine ticket activity and unnecessary workflow detail are minimized.

The goal is a concise, decision-ready view of the project rather than another Jira activity report.

---

## Client Reporting

Baseline Guard turns Jira evidence into clear, client-ready project reporting.

Client reporting focuses on information appropriate for external stakeholders, including:

- Current project position
- Relevant progress and commitments
- Commitments requiring attention
- Client-relevant risks
- Important checkpoints
- Decisions requiring client involvement
- Proposed follow-through
- Known evidence limitations

Client reports are designed to communicate project reality without requiring clients to understand internal Jira workflows.

Internal operational information that is not appropriate for a client audience is excluded from the client reporting context.

This includes internal details such as assignees, labels, sprint names, priority levels, internal dependencies, and internal-only risks.

---

## Internal Team Reporting

Internal reporting gives delivery teams a detailed, evidence-backed view of project health.

Internal reporting can surface:

- Delivery risk
- Evidence deficiencies
- Operational concerns
- Items requiring attention
- Relevant Jira context
- Owners and priorities
- Sprint and delivery context
- Proposed remediation
- Required next actions

When Baseline Guard cannot produce a defensible assessment, internal reporting helps explain what evidence is missing and what the team needs to address.

This makes a **NOT ASSESSABLE** result actionable rather than simply reporting that information is unavailable.

---

## Risks and Commitments

Baseline Guard identifies meaningful delivery signals supported by available Jira evidence.

Depending on the project and evidence available, an assessment may surface:

- Overdue commitments
- Upcoming commitments
- Blocked work
- Delivery risks
- Items requiring attention
- Relevant ownership information
- Important checkpoints
- Evidence limitations

Baseline Guard is designed to prioritize meaningful project signals rather than reproduce every Jira issue in a status report.

---

## Decisions

When available Jira evidence indicates that a decision may be required, Baseline Guard can surface that decision for attention.

Depending on the evidence available, a decision item may include:

- The decision question
- Why attention is required
- Relevant timing
- Available options or tradeoffs
- Consequences
- Supporting Jira evidence

Baseline Guard does not manufacture a decision when the Jira evidence does not support one.

---

## Recommendations and Proposed Actions

Where supported by the evidence, Baseline Guard may identify recommendations, proposed actions, or remediation.

Recommendations are presented as recommendations rather than established facts.

This distinction is intentional.

Baseline Guard separates:

**What the Jira evidence establishes**

from

**What may be an appropriate response to that evidence**

This helps teams use Baseline Guard for decision support without presenting proposed actions as facts.

---

## Missing Evidence

Missing information can itself be an important project signal.

Baseline Guard is deliberately conservative when Jira does not contain enough information to support a conclusion.

Instead of inventing missing facts or presenting unsupported certainty, Baseline Guard identifies relevant evidence deficiencies and explains their effect on the assessment.

Insufficient evidence may result in a **NOT ASSESSABLE** determination.

The principle is simple:

**No evidence, no invented certainty.**

---

## Data Access and Permissions

Baseline Guard is designed around least-privilege access.

The app uses Jira's **read:jira-work** permission to read project and issue information required to generate assessments and reports.

Baseline Guard:

- Uses read-only Jira access.
- Does not modify Jira issues.
- Does not require Jira write permissions.
- Does not request the `read:jira-user` scope.
- Does not require users to provide external AI API keys.
- Does not fetch Jira comments.
- Respects the Jira permissions of the user generating the assessment.

Jira requests are made in the context of the current user.

Baseline Guard cannot be used to access Jira project or issue information that the current Jira user is not permitted to access.

---

## Jira Data Used

Depending on the project, reporting period, and reporting audience, Baseline Guard may evaluate Jira information including:

- Issue summary
- Status
- Status category
- Issue type
- Priority
- Created date
- Updated date
- Resolution date
- Due date
- Labels
- Assignee
- Parent issue
- Sprint information

Baseline Guard requests the Jira fields required for assessment rather than requesting all available issue fields.

**Jira comments are not fetched or used as assessment evidence.**

Information included in the generated report can vary according to the selected reporting audience.

---

## AI-Assisted Analysis

Baseline Guard uses Atlassian's native **Forge LLM** capability to assist with structured analysis and reporting.

Report generation runs within the Atlassian Forge environment.

Baseline Guard does not require customers to provide external AI API keys and does not send Jira issue data to an external AI provider operated by Baseline Guard.

AI-generated output is constrained by the Jira evidence supplied to the assessment.

Baseline Guard validates evidence references against the Jira issues available to the assessment so unsupported issue references cannot silently become evidence for a conclusion.

Facts and interpretations are distinguished where appropriate.

Recommendations are identified as recommendations rather than facts.

Baseline Guard is not designed to produce a generic AI summary.

It is designed to produce an evidence-backed project assessment that stakeholders can understand, evaluate, and defend.

---

## Data Storage and Retention

Baseline Guard assessments are generated on demand from Jira data.

**Baseline Guard does not persist generated assessments or Jira issue content as a separate customer data store.**

Jira issue content is not intentionally written to application storage.

Generated assessment content is not written back to Jira.

Local interactions or edits to a generated report are page-local and are not persisted by Baseline Guard.

Generating a new assessment evaluates the Jira evidence available at the time of generation.

Baseline Guard does not intentionally log Jira issue content.

For complete information about data handling, processing, and privacy, see the **Baseline Guard Privacy Policy**.

---

## Read-Only Operation

Baseline Guard is an assessment and reporting layer for Jira.

Generating or reviewing an assessment does not change:

- Jira issue status
- Assignees
- Priorities
- Due dates
- Issue content
- Project configuration

Baseline Guard does not become another project system of record.

**Jira remains the source of project evidence.**

---

## Evidence Limitations

Baseline Guard can only evaluate evidence available in Jira and accessible to the current user.

The quality and completeness of an assessment therefore depend on the quality and completeness of the underlying Jira data.

Missing, outdated, or incomplete Jira information may:

- Reduce evidence confidence
- Limit conclusions
- Produce evidence deficiencies
- Prevent some risks or commitments from being identified
- Result in a NOT ASSESSABLE determination

Baseline Guard surfaces known evidence limitations where appropriate rather than treating incomplete information as complete.

---

## Troubleshooting

### No projects appear in the project selector

Confirm that your Jira account has access to the projects you expect to assess.

Baseline Guard respects the permissions of the Jira user accessing the app.

---

### The assessment is NOT ASSESSABLE

This is not necessarily an application error.

A NOT ASSESSABLE result means the available Jira evidence does not support a sufficiently defensible assessment.

Review the evidence gaps or remediation information presented by Baseline Guard to determine what Jira information needs attention.

---

### The assessment contains limited information

Baseline Guard can only evaluate evidence available in Jira and accessible to the current user.

Incomplete Jira records or a reporting period containing limited activity may therefore produce a more limited assessment.

---

### The report does not show information I expected

Confirm that the information exists in Jira, falls within the selected reporting context, and is visible to your Jira account.

The selected reporting audience can also affect which information is included.

Client reports intentionally exclude certain internal operational details.

---

### Jira information changed after an assessment was generated

Baseline Guard assessments reflect Jira evidence available when the assessment is generated.

If project information has changed, generate a new assessment to evaluate the current Jira evidence.

---

### An assessment cannot be generated

Try generating the assessment again.

If the problem continues, contact Baseline Guard Support with a description of the problem and any error message displayed by the application.

Please do not send confidential Jira issue content through an unapproved support channel.

---

## Security and Privacy

Baseline Guard is built on Atlassian Forge and designed to minimize unnecessary access to customer information.

The product is designed around the following principles:

- Least-privilege Jira access
- Read-only operation
- Evidence-based analysis
- Explicit Jira field access
- No Jira comments used for assessment
- No persistence of Jira issue content as a separate customer data store
- No intentional logging of Jira issue content
- Clear separation between facts, interpretations, and recommendations
- Jira permission enforcement through the current user's access

For complete information about data handling, processing, and privacy, see the **Baseline Guard Privacy Policy**.

---

## Support

Baseline Guard is a supported commercial Atlassian Marketplace application.

For installation issues, assessment-generation problems, or questions about using Baseline Guard, contact **Baseline Guard Support**.

When contacting support, include:

- A description of the problem
- The action you were attempting
- Any error message displayed by Baseline Guard

Please do not send confidential Jira issue content unless specifically requested through an approved support channel.
