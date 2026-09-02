# Baseline Guard for Jira — Customer Documentation

**Documentation** · [Support](support.html) · [Privacy Policy](privacy.html) · [End User Terms](terms.html)

Baseline Guard is an evidence-based project reporting app for Jira Cloud. It
checks whether a Jira project contains enough evidence to support a project
status, then produces a report for an Executive, Client, or Internal audience.
Every audience uses the same underlying Jira facts and determination.

## Supported environment

Baseline Guard supports Jira Cloud and is installed through the Atlassian
Marketplace. It runs inside Jira on Atlassian Forge. Reports and documentation
are currently provided in English.

Baseline Guard reads supported Jira information available to the person using
the app. It does not update Jira issues or automatically correct project data.

## Installation and access

1. A Jira Cloud administrator installs Baseline Guard from its Atlassian
   Marketplace listing and starts an available trial or subscription.
2. Review and accept the permissions shown by Atlassian for the Jira site.
3. In Jira, open **Apps**, then select **Baseline Guard**.

You need permission to view a Jira project before you can assess it. Baseline
Guard only lists projects available to your Jira account. An active Marketplace
trial or subscription is required to run and retrieve assessments.

## Run an assessment

1. Under **Project**, choose the Jira project you want to assess.
2. Under **Reporting period**, choose **Last 7 days**, **Last 14 days**,
   **Last 30 days**, **Current sprint**, or **Custom range**. For a custom
   range, enter both a start and an end date.
3. Select **Executive**, **Client**, or **Internal** under **Audience**.
4. Select **Run assessment** and wait while Baseline Guard reads the available
   Jira evidence and prepares the report.
5. Review the determination, readiness, health signals, audience brief, and
   evidence limitations.
6. Expand **Evidence & audit trail** when you need source details and
   provenance.
7. Select **Copy report** to copy the report shown for the selected audience.

Use **Run again** to produce a new assessment after Jira evidence or report
choices change.

## Audience modes

The status, confidence, trend, readiness, health counts, and source evidence do
not change between audiences. The presentation changes so the same facts are
useful to different readers.

- **Executive** emphasizes the current determination, decision-relevant
  attention items, evidenced decisions, and concise proposed next actions.
- **Client** presents an external-facing status brief, relevant commitments and
  impacts that Jira establishes, and any evidenced clarification or decision
  needed from the client. Internal operational detail is limited.
- **Internal** emphasizes operational priorities, workflow state, ownership
  presence, blockers, due dates, decisions, and Jira-backed delivery actions.

If a project is not assessable, each audience receives an appropriate
explanation of the missing evidence and the Jira-backed step needed to restore
assessability. No audience converts a non-assessable result into a project
health status.

## Project-status determinations

- **ON TRACK** means the supported Jira evidence satisfies the conditions for
  an on-track project status.
- **AT RISK** means the evidence identifies delivery exposure that requires
  attention.
- **OFF TRACK** means the evidence identifies material current delivery
  exposure.
- **NOT ASSESSABLE** means Baseline Guard cannot issue a defensible project
  health status from the available evidence. It is not an on-track, at-risk,
  or off-track result.

Baseline Guard reports what the supported Jira evidence establishes at the
time of assessment. Its reports are decision support, not forecasts,
guarantees, or professional advice.

## Four different report concepts

These concepts answer different questions and should be read separately:

- **Assessment readiness:** Are all mandatory evidence prerequisites
  established? Full readiness means a status may be assessed; it does not mean
  the project is healthy.
- **Project health:** What status does the current supported evidence justify?
  This is the ON TRACK, AT RISK, or OFF TRACK determination.
- **Evidence confidence:** How complete and consistent is the evidence that
  supports the current determination? Confidence is not a health rating.
- **Trend:** Does comparable prior-period evidence establish a direction of
  change? A current status may be available even when trend is
  **NOT ASSESSABLE** because no comparable prior period exists.

## The eight evidence prerequisites

Before issuing a project health status, Baseline Guard checks eight mandatory
conditions in a fixed order:

1. **Accountable owner:** Jira identifies a project lead who is accountable for
   the project.
2. **Delivery outcome or milestone:** At least one Epic description states an
   outcome or milestone.
3. **Target date:** Jira contains a version release date or an issue or Epic due
   date.
4. **Enumerable work scope:** The project contains a readable, non-empty body
   of work that can be assessed.
5. **Work ownership:** At least one issue or Epic has an assignee established in
   Jira.
6. **Active work signal:** Jira contains measurable activity in the reporting
   scope.
7. **Dependency or blocker declaration:** Jira records a supported blocker or
   dependency signal, or explicitly declares that none exist.
8. **Reporting cadence and status ownership:** Jira contains recently updated
   work and an established person responsible for project status.

The report shows which conditions are established, proven deficient, or cannot
be verified from the Jira evidence available to the app. A missing or
unverifiable prerequisite prevents Baseline Guard from inventing a health
status.

## Active delivery signals

Baseline Guard interprets these signals from active Jira work:

- **Overdue:** an active work item has a Jira due date before the assessment
  date.
- **Blocked:** an active work item has a supported Jira blocked status or
  supported blocking relationship.
- **Due soon:** an active work item has a Jira due date from the assessment date
  through the next seven days.

Completed work is excluded from overdue, due-soon, active-blocker, attention,
decision, and proposed-action lists because it is no longer active delivery
exposure. Baseline Guard uses Jira resolution evidence and Jira's normal Done
classification to recognize completed work. If a workflow labels an unresolved
issue **Blocked** but maps that status to Jira's Done category, Baseline Guard
keeps it as an active blocker and explains the workflow inconsistency in the
report.

## Correct missing Jira evidence

When a project is not assessable, read the named evidence gap or deficiency in
the report. Correct Jira only when the project has a real fact or declaration
to record. Common examples include:

- assigning the project lead or relevant work;
- adding an outcome or milestone to an Epic description;
- recording a real target or due date;
- making the project scope readable and non-empty;
- recording current project activity; or
- recording the true blocker or dependency state, including an explicit
  declaration that no blockers exist when that is accurate.

Do not add placeholder information merely to obtain a preferred status. After
the Jira evidence accurately reflects the project, run a new assessment.

## Evidence and audit trail

The main brief uses plain language for the selected audience. Expand
**Evidence & audit trail** to review the determination basis, evidence facts,
interpretations, proposed actions, Jira source keys, evidence limitations, and
provenance. Source keys link back to the Jira issues available to you.

Facts come from supported Jira fields. Interpretations are deterministic
conclusions based on those facts. Proposed actions are clearly labeled and do
not create Jira changes. Baseline Guard does not invent owners, dates,
dependencies, impacts, or consequences that Jira does not establish.

The copied report contains the same authoritative determination and evidence
shown on screen for the selected audience.

## Data handling and privacy

Baseline Guard runs on Atlassian Forge and processes selected Jira information
to provide the assessment. The app does not operate an independently hosted
external backend for customer Jira data and does not update Jira. For the full
description of accessed information, storage, retention, authorization, and
privacy requests, read the [Baseline Guard Privacy Policy](privacy.html).

## Terms

Installation and use of Baseline Guard are governed by the
[Baseline Guard End User Terms](terms.html) and any applicable Atlassian
Marketplace subscription terms.

## Support

Visit the [Baseline Guard Support page](support.html) to open a support request,
report a bug, request a feature, or contact us privately about an account,
privacy, or security matter.

Do not send report bodies, passwords, access tokens, or confidential Jira issue
content in an initial support request.
