# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, assess, manage, monitor, and communicate risks and dependencies throughout the project lifecycle. This document provides comprehensive guidance for proactive risk management and effective stakeholder communication.

## Risk Register

Maintain a comprehensive risk register with the following fields:

| Field | Description | Example Values |
|-------|-------------|----------------|
| **Risk ID** | Unique identifier | RISK-001, RISK-002 |
| **Category** | Type of risk | Technical, Schedule, Resource, External, Quality |
| **Description** | Clear statement of the risk | "Third-party API may have rate limits that impact peak usage" |
| **Impact** | Effect if risk occurs | High / Medium / Low |
| **Likelihood** | Probability of occurrence | High / Medium / Low |
| **Risk Score** | Impact × Likelihood (numeric) | 1-9 (calculated using scores below) |
| **Owner** | Person responsible for monitoring | Name or role |
| **Mitigation Plan** | Actions to reduce likelihood or impact | Specific steps to address risk |
| **Contingency Plan** | Backup plan if risk occurs | What to do if mitigation fails |
| **Status** | Current state | Open / Monitoring / Mitigated / Closed |
| **Date Identified** | When risk was logged | YYYY-MM-DD |
| **Last Updated** | Most recent review date | YYYY-MM-DD |

### Risk Scoring Matrix

Calculate risk score by multiplying Impact and Likelihood scores:

**Impact Scores:**
- **High (3)**: Critical impact on project success, timeline, or budget (>20% deviation)
- **Medium (2)**: Moderate impact requiring workarounds or adjustments (5-20% deviation)
- **Low (1)**: Minor impact with minimal project effect (<5% deviation)

**Likelihood Scores:**
- **High (3)**: Probable to occur (>60% chance)
- **Medium (2)**: Possible to occur (30-60% chance)
- **Low (1)**: Unlikely to occur (<30% chance)

**Risk Priority:**
- **Critical (7-9)**: Immediate attention required, escalate to leadership
- **High (4-6)**: Active monitoring and mitigation planning required
- **Low (1-3)**: Track and review periodically

## Risk Lifecycle

### 1. Risk Identification

**When to identify risks:**
- During project initiation and planning phases
- At sprint/iteration planning meetings
- During daily standups when issues arise
- In weekly team syncs and risk reviews
- When dependencies or external factors change
- After incidents or retrospectives

**How to identify risks:**
- Brainstorming sessions with cross-functional team
- Review similar past projects for lessons learned
- Dependency mapping exercises
- Technical architecture reviews
- Stakeholder interviews and feedback
- SWOT analysis (Strengths, Weaknesses, Opportunities, Threats)

**Common risk categories:**
- **Technical**: Technology limitations, integration challenges, performance issues
- **Schedule**: Timeline constraints, dependency delays, resource availability
- **Resource**: Team availability, skill gaps, budget constraints
- **External**: Third-party dependencies, vendor reliability, market changes
- **Quality**: Testing gaps, technical debt, compliance requirements
- **Communication**: Stakeholder misalignment, unclear requirements, information silos

### 2. Risk Assessment

**Assessment process:**
1. Document the risk clearly and concisely
2. Determine impact using the scoring matrix (High/Medium/Low)
3. Estimate likelihood using historical data and expert judgment
4. Calculate risk score (Impact × Likelihood)
5. Assign an owner responsible for monitoring
6. Categorize the risk type

**Assessment questions:**
- What is the worst-case scenario if this risk occurs?
- How likely is this to happen based on current conditions?
- What are the warning signs that this risk is materializing?
- Who is best positioned to monitor and respond to this risk?
- Are there dependencies or related risks?

### 3. Risk Mitigation

**Mitigation strategies:**
- **Avoid**: Change plans to eliminate the risk entirely
- **Reduce**: Take actions to decrease likelihood or impact
- **Transfer**: Shift responsibility (e.g., insurance, vendor contracts)
- **Accept**: Acknowledge the risk and prepare contingency plans

**Mitigation plan components:**
- Specific actions to reduce likelihood or impact
- Timeline for implementing mitigation actions
- Resources required for mitigation
- Success criteria for mitigation
- Contingency plan if primary mitigation fails

**Example mitigation plans:**
- Risk: "API rate limits may impact peak usage"
  - Mitigation: Implement request caching and rate limiting on client side
  - Contingency: Negotiate higher rate limits with vendor, implement queue system
- Risk: "Key developer unavailable during critical sprint"
  - Mitigation: Cross-train two additional developers on critical components
  - Contingency: Adjust sprint scope or extend timeline

### 4. Risk Monitoring

**Monitoring cadence:**
- **Daily**: Critical risks (score 7-9) reviewed in standup
- **Weekly**: All active risks reviewed in team sync
- **Monthly**: Full risk register review and cleanup
- **Ad-hoc**: When risk triggers or warning signs appear

**Monitoring activities:**
- Check risk triggers and warning indicators
- Update risk status and likelihood as conditions change
- Document new information or developments
- Escalate risks that are materializing
- Close risks that are no longer relevant
- Identify new risks as they emerge

**Risk status definitions:**
- **Open**: Newly identified, mitigation planning in progress
- **Monitoring**: Mitigation plan in place, actively tracking
- **Mitigated**: Actions taken, risk reduced to acceptable level
- **Occurred**: Risk has materialized, executing contingency plan
- **Closed**: Risk no longer applicable or fully resolved

## Dependency Management

Dependencies are external factors or other work items that your project relies on. Proactive dependency management prevents delays and surprises.

### Dependency Types
- **Internal Team**: Dependencies on other teams within the organization
- **External Vendor**: Third-party services, APIs, or tools
- **Technical**: Infrastructure, platforms, or technology prerequisites
- **Resource**: People, budget, or equipment availability
- **Regulatory**: Compliance, legal, or approval requirements

### Dependency Tracking

Maintain a dependency register with:
- **Dependency ID**: Unique identifier
- **Description**: What is needed and from whom
- **Type**: Internal, External, Technical, Resource, Regulatory
- **Owner**: Person coordinating this dependency
- **Dependent Team/Vendor**: Who provides this
- **Required By Date**: When this is needed
- **Status**: Requested / In Progress / Blocked / Resolved
- **Impact if Delayed**: Effect on project timeline
- **Mitigation**: Backup plan if dependency is delayed

### Dependency Management Process
1. **Identify dependencies** during project planning
2. **Document** in dependency register with clear ownership
3. **Communicate** requirements to dependent teams/vendors early
4. **Track** status in weekly syncs and update register
5. **Escalate** blocked or at-risk dependencies immediately
6. **Validate** when dependencies are delivered
7. **Update** project plans if dependencies shift

## Stakeholder Communication

Effective communication ensures alignment, manages expectations, and builds trust with stakeholders.

### Stakeholder Identification

Create a stakeholder matrix identifying:
- **Name/Group**: Individual or team
- **Interest Level**: High / Medium / Low
- **Influence Level**: High / Medium / Low
- **Communication Needs**: What information they need
- **Preferred Channel**: Email, meetings, dashboards, etc.
- **Frequency**: Daily, weekly, monthly, milestone-based

### Communication Matrix

| Stakeholder Type | Information Needs | Frequency | Channel | Owner |
|-----------------|-------------------|-----------|---------|-------|
| **Executive Sponsors** | High-level status, risks, decisions needed | Monthly or milestone-based | Executive summary email or brief | Project Manager |
| **Product Leadership** | Progress, scope changes, resource needs | Weekly | Sync meeting + written update | Product Manager |
| **Engineering Teams** | Technical details, dependencies, blockers | Daily/Weekly | Standup, Slack, project board | Tech Lead or Scrum Master |
| **Dependent Teams** | Integration points, timelines, API changes | Weekly or as needed | Email + sync meetings | Project Manager |
| **Support/Operations** | Feature releases, known issues, documentation | Pre-release + at release | Release notes, training session | Release Manager |
| **End Users/Customers** | New features, changes, benefits | At release | Product announcements, docs | Product Manager |

### Single Source of Truth

Maintain one authoritative location for project status:
- Project README or wiki page
- Project board (e.g., GitHub Projects)
- Shared document with status updates
- Team dashboard with metrics

Update this source regularly and direct all stakeholders to it for current information.

## Communication Templates

### Weekly Status Update Template

**Subject**: [Project Name] - Week of [Date] Status Update

**Progress This Week:**
- [Completed item 1 with impact/value]
- [Completed item 2 with impact/value]
- [Metrics or achievements]

**Next Week's Focus:**
- [Planned work item 1]
- [Planned work item 2]
- [Key milestones or deliverables]

**Risks & Blockers:**
- **[Risk ID]**: [Description] - Impact: [H/M/L] - Mitigation: [Plan]
- **Blocker**: [Description] - Need: [What's required to unblock]

**Decisions Needed:**
- [Decision 1 with context and options]
- [Decision 2 with timeline]

**Metrics:**
- Sprint velocity: [X points/items completed vs Y planned]
- Quality: [Test coverage %, bugs found/fixed]
- Timeline: [On track / X days ahead/behind]

**Asks/Support Needed:**
- [Specific request 1]
- [Specific request 2]

---

### Project Kickoff Communication Template

**Subject**: [Project Name] - Kickoff & Charter

**Project Overview:**
- **Problem Statement**: [What problem are we solving?]
- **Objective**: [SMART goal]
- **Success Metrics**: [How we'll measure success]

**Team & Roles:**
- Product Owner: [Name]
- Project Manager: [Name]
- Tech Lead: [Name]
- [Other key roles]

**Timeline:**
- Start Date: [Date]
- Key Milestones: [M1: Date, M2: Date]
- Target Release: [Date]

**Communication Plan:**
- Standup: [Days/Time]
- Sprint Review: [Frequency/Day]
- Stakeholder Updates: [Frequency]
- Team Channel: [Link to Slack/Teams]

**Next Steps:**
- [Action 1] - Owner: [Name] - Due: [Date]
- [Action 2] - Owner: [Name] - Due: [Date]

---

### Milestone Completion Update Template

**Subject**: [Project Name] - [Milestone Name] Completed

**Milestone Achievement:**
[1-2 sentences on what was accomplished]

**Key Deliverables:**
- [Deliverable 1 with link or description]
- [Deliverable 2 with link or description]
- [Deliverable 3 with link or description]

**Metrics/Outcomes:**
- [Metric 1: Value]
- [Metric 2: Value]
- [User feedback or other success indicators]

**Learnings:**
- What went well: [Insight]
- What to improve: [Insight]

**Next Steps:**
- Upcoming Milestone: [Name] - Target: [Date]
- Focus Areas: [Key priorities]

**Thank Yous:**
[Recognize team members and contributors]

---

### Incident Communication Template

**Subject**: [INCIDENT] [Severity] - [Brief Description]

**Incident Summary:**
- **Status**: [Investigating / Mitigating / Resolved]
- **Severity**: [Critical / High / Medium / Low]
- **Impact**: [What's affected and how many users]
- **Started**: [Time]
- **Detected**: [Time]

**What Happened:**
[Clear, concise description of the incident]

**Current Actions:**
- [Action being taken 1]
- [Action being taken 2]
- [People involved and their roles]

**Expected Timeline:**
- **Next Update**: [Time]
- **Estimated Resolution**: [Time or "Unknown - investigating"]

**Mitigation/Workaround:**
[If available, what users can do to avoid/minimize impact]

**Follow-up:**
- Post-incident review scheduled: [Date/Time]
- Incident report will be shared: [Date]

**Contact:**
For questions: [Contact person/channel]

---

### Blocker Escalation Template

**Subject**: [BLOCKER] [Project Name] - [Brief Description]

**Blocker Description:**
[Clear description of what is blocked and why]

**Impact:**
- **Timeline Impact**: [X days delay / Risk to milestone]
- **Scope Impact**: [Features affected]
- **Team Impact**: [Team members blocked, % of capacity]

**What We've Tried:**
- [Attempt 1 - result]
- [Attempt 2 - result]

**What We Need:**
[Specific ask - decision, resource, approval, information, etc.]

**Options/Recommendations:**
1. [Option 1] - Pros: [X] / Cons: [Y] / Timeline: [Z]
2. [Option 2] - Pros: [X] / Cons: [Y] / Timeline: [Z]

**Decision Needed By:**
[Date/Time] - [Reason for urgency]

**Follow-up:**
[Who will track this and report back]

---

### Dependency Request Template

**Subject**: [DEPENDENCY] [Project Name] needs [What] from [Team/Vendor]

**Request Summary:**
[1-2 sentence description of what's needed]

**Context:**
- **Our Project**: [Brief description]
- **Why We Need This**: [Business/technical justification]
- **How We'll Use It**: [Integration or usage details]

**Requirements:**
- [Specific requirement 1]
- [Specific requirement 2]
- [Acceptance criteria]

**Timeline:**
- **Need By**: [Date]
- **Our Dependent Milestone**: [What we're blocking]
- **Impact if Delayed**: [Consequences]

**Collaboration:**
- **Our Point of Contact**: [Name]
- **Preferred Communication**: [Channel/meeting cadence]
- **Documentation/Specs**: [Link to detailed requirements]

**Next Steps:**
- [Requested confirmation of feasibility]
- [Proposed sync meeting to discuss]

---

### Release Announcement Template

**Subject**: [Project Name] - [Release Version] Now Available

**Release Highlights:**
[2-3 sentences on the most important changes]

**What's New:**
- **[Feature 1]**: [Brief description and benefit]
- **[Feature 2]**: [Brief description and benefit]
- **[Improvement 3]**: [Brief description and benefit]

**Getting Started:**
- Documentation: [Link]
- Tutorial/Demo: [Link]
- Support Channel: [Link]

**Breaking Changes:**
[If any, describe what changed and migration steps]

**Known Issues:**
[If any, list with workarounds]

**Rollout Plan:**
- Phase 1: [User group] - [Date]
- Phase 2: [User group] - [Date]
- Full availability: [Date]

**Feedback:**
We'd love your feedback! [How to provide feedback]

**Thank You:**
[Recognize contributors and thank users]

## Escalation Paths

Clear escalation paths ensure issues are resolved quickly at the appropriate level.

### Standard Escalation Hierarchy

**Level 0 - Team Level** (Response: Immediate)
- **When**: Day-to-day technical blockers, clarification questions
- **Who**: Team members, Tech Lead, Scrum Master
- **Channel**: Daily standup, team chat, direct communication
- **Resolution time**: Same day

**Level 1 - Project Management** (Response: Same day)
- **When**: Risks affecting timeline, resource needs, cross-team coordination
- **Who**: Project Manager, Product Owner
- **Channel**: Weekly sync, direct outreach, project status meeting
- **Resolution time**: 1-2 days

**Level 2 - Leadership** (Response: 1-2 days)
- **When**: Budget issues, significant scope changes, resource conflicts
- **Who**: Product Lead, Engineering Manager, Director
- **Channel**: Email with summary, scheduled meeting
- **Resolution time**: 3-5 days

**Level 3 - Executive/Sponsor** (Response: As needed)
- **When**: Strategic decisions, major timeline impact, organizational dependencies
- **Who**: VP, Sponsor, Executive team
- **Channel**: Executive brief, escalation meeting
- **Resolution time**: 1-2 weeks

### Escalation Triggers

Escalate immediately when:
- **Critical blocker** preventing team progress for >1 day
- **Risk materialization** that impacts key milestones or budget
- **Dependency failure** from external team or vendor
- **Resource shortage** affecting ability to deliver
- **Scope dispute** requiring product or business decision
- **Security or compliance** issue discovered
- **Production incident** with user impact

### Escalation Best Practices

1. **Document first**: Clearly describe the issue, impact, and what's been tried
2. **Bring options**: Propose 2-3 solutions with pros/cons
3. **Specify needs**: Be clear about what decision or resource is needed
4. **Set deadline**: Explain timeline urgency and consequences of delay
5. **Follow up**: Track the escalation and confirm resolution
6. **Close the loop**: Update stakeholders on outcome

### Special Escalation Paths

**Security Incidents:**
1. Notify Security on-call immediately (page if needed)
2. Follow security incident response runbook
3. Inform Project Manager and Product Lead
4. Do NOT communicate externally until cleared by Security
5. Document timeline and actions in incident log

**Production Outages:**
1. Trigger incident response and notify on-call
2. Update status page with user-facing communication
3. Engage Release Manager and Tech Lead
4. Execute rollback if needed
5. Schedule post-incident review

**Data Privacy Issues:**
1. Notify Privacy Officer and Legal immediately
2. Halt related activities until cleared
3. Document data exposure scope
4. Follow data breach response protocol
5. Prepare user notifications if required

**Vendor/Partner Issues:**
1. Attempt direct resolution with vendor contact
2. Escalate to Project Manager if unresolved in 24 hours
3. Engage procurement or partnerships team if needed
4. Document SLA breaches and impact
5. Activate contingency plans if available

## Communication Best Practices

### Dos
- ✅ Be clear, concise, and specific
- ✅ Use data and examples to illustrate points
- ✅ Provide context and impact in updates
- ✅ Share both successes and challenges transparently
- ✅ Use appropriate channels for different stakeholders
- ✅ Follow up on commitments and action items
- ✅ Document decisions and their rationale
- ✅ Respect people's time with focused, relevant updates

### Don'ts
- ❌ Bury important information in long messages
- ❌ Send urgent information only via email
- ❌ Use jargon or acronyms with non-technical stakeholders
- ❌ Surprise stakeholders with bad news
- ❌ Over-communicate to the point of noise
- ❌ Share different status with different stakeholders
- ❌ Skip updates when there's "nothing new"
- ❌ Communicate blame or negativity without solutions

## Communication Checklist

Use this checklist to ensure effective project communication:

### Project Initiation
- [ ] Stakeholder matrix created and reviewed
- [ ] Kickoff communication sent to all stakeholders
- [ ] Communication channels established (chat, email lists, meeting invites)
- [ ] Single source of truth for status identified
- [ ] Escalation paths documented and shared

### During Execution
- [ ] Weekly status updates sent on consistent schedule
- [ ] Risk register reviewed and communicated weekly
- [ ] Dependency status tracked and escalated as needed
- [ ] Decision log maintained and accessible
- [ ] Milestone achievements celebrated and announced

### At Release
- [ ] Release notes prepared and reviewed
- [ ] Support team briefed on changes
- [ ] Stakeholders notified of rollout plan
- [ ] Success metrics tracking confirmed
- [ ] Feedback channels established

### Project Closure
- [ ] Final status update sent to all stakeholders
- [ ] Retrospective conducted and documented
- [ ] Lessons learned shared with broader organization
- [ ] Thank you notes sent to contributors
- [ ] Project artifacts archived appropriately
