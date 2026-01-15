# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Product Owner

### Role Summary
Product Owners represent the voice of the customer and stakeholders. They define and prioritize the product backlog, ensuring maximum value delivery while balancing business needs and technical constraints.

### Responsibilities
- Maintain and prioritize the product backlog
- Define user stories with clear acceptance criteria
- Make trade-off decisions on scope and features
- Accept or reject completed work based on acceptance criteria
- Collaborate with stakeholders to gather requirements
- Ensure the team understands backlog items

### Goals
- Maximize return on investment (ROI) and business value
- Ensure clear and actionable backlog items
- Maintain alignment between development and business objectives
- Deliver features that meet customer needs

### Typical Communication
- Backlog refinement sessions with development team
- Sprint planning and review meetings
- Daily availability for clarifications on requirements
- Regular stakeholder updates on product progress

### Interactions with Other Roles
- **Developers**: Clarify requirements and acceptance criteria, answer questions
- **Product Managers**: Align on product vision and strategic priorities
- **Scrum Master**: Collaborate on sprint planning and backlog health
- **QA Lead**: Define acceptance criteria and validation approaches
- **Stakeholders**: Gather feedback and manage expectations

---

## Scrum Master

### Role Summary
Scrum Masters facilitate agile practices and remove impediments that block team progress. They coach the team on agile principles and ensure processes are followed effectively.

### Responsibilities
- Facilitate agile ceremonies (standups, planning, retrospectives, reviews)
- Remove blockers and impediments for the team
- Coach team members on agile practices and principles
- Shield the team from external disruptions
- Track and improve team velocity and process health
- Foster continuous improvement culture

### Goals
- Enable high team productivity and autonomy
- Build a self-organizing, collaborative team
- Ensure consistent application of agile practices
- Continuously improve team processes and efficiency

### Typical Communication
- Daily facilitation of standup meetings
- Weekly metrics reviews and process improvements
- Ad-hoc coaching and impediment resolution
- Retrospective facilitation and action tracking

### Interactions with Other Roles
- **Developers**: Remove blockers, coach on practices, facilitate collaboration
- **Product Owner**: Support backlog refinement and sprint planning
- **Project Manager**: Coordinate on dependencies and resource needs
- **Release Manager**: Align on delivery timelines and readiness

---

## Stakeholder Representative

### Role Summary
Stakeholder Representatives advocate for specific business units, user groups, or organizational interests. They provide input on requirements, validate solutions, and ensure outcomes meet stakeholder needs.

### Responsibilities
- Communicate stakeholder needs and priorities to the team
- Participate in planning and review sessions
- Provide feedback on features and deliverables
- Validate that solutions meet stakeholder requirements
- Escalate concerns or issues to appropriate leadership
- Support user acceptance testing and rollout activities

### Goals
- Ensure delivered solutions meet stakeholder expectations
- Maintain clear communication between teams and stakeholders
- Identify risks and opportunities early
- Support successful adoption and change management

### Typical Communication
- Sprint reviews and milestone demonstrations
- Feedback sessions and user acceptance testing
- Monthly stakeholder steering committee meetings
- Ad-hoc consultations on requirements and priorities

### Interactions with Other Roles
- **Product Owner**: Provide requirements and validate backlog priorities
- **Product Manager**: Share business context and success metrics
- **Project Manager**: Review status, risks, and timeline implications
- **QA Lead**: Participate in acceptance testing and validation
- **Release Manager**: Coordinate rollout and adoption activities

---

## Release Manager

### Role Summary
Release Managers coordinate and oversee the release process from planning through production deployment. They ensure releases are well-planned, properly tested, and safely deployed with minimal risk.

### Responsibilities
- Plan and schedule releases across multiple teams
- Coordinate release activities and dependencies
- Manage release readiness reviews and go/no-go decisions
- Ensure compliance with release policies and standards
- Coordinate rollback procedures when needed
- Track and report on release metrics and post-deployment health
- Maintain release calendars and communicate schedules

### Goals
- Deliver high-quality releases with minimal production incidents
- Reduce deployment cycle time and increase deployment frequency
- Ensure predictable, repeatable release processes
- Minimize production risks through proper planning and validation

### Typical Communication
- Release planning meetings with engineering and product teams
- Release readiness reviews and go/no-go decision meetings
- Post-deployment status updates and metrics reviews
- Coordination with support and operations teams

### Interactions with Other Roles
- **Developers**: Review release contents and deployment procedures
- **QA Lead**: Validate testing completion and release readiness
- **Project Manager**: Align release timelines with project milestones
- **Product Manager**: Coordinate release communications and announcements
- **Stakeholders**: Communicate release schedules and impacts

---

## QA Lead

### Role Summary
QA Leads define and oversee quality assurance strategies, ensuring that delivered software meets quality standards and acceptance criteria. They coordinate testing activities and advocate for quality throughout the development lifecycle.

### Responsibilities
- Define QA strategy and test approach for projects
- Create and maintain test plans and test cases
- Coordinate manual and automated testing activities
- Lead acceptance testing and sign-off processes
- Identify quality risks and advocate for bug fixes
- Establish and monitor quality metrics
- Mentor team members on testing best practices

### Goals
- Ensure high product quality and reliability
- Minimize production defects and customer-reported issues
- Improve test coverage and automation
- Reduce testing cycle time while maintaining quality

### Typical Communication
- Daily coordination with developers on testing needs
- Weekly quality metrics reviews and risk assessments
- Sprint planning for test coverage and approach
- Release readiness reviews with Release Manager

### Interactions with Other Roles
- **Developers**: Clarify acceptance criteria, report bugs, collaborate on testability
- **Product Owner**: Validate acceptance criteria and feature completeness
- **Release Manager**: Provide test sign-off and quality status for releases
- **Scrum Master**: Participate in retrospectives to improve quality processes
- **Project Manager**: Report on quality risks and testing progress

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

## Role Interaction Matrix

Understanding how roles collaborate is critical for project success. Below is a quick reference for key interactions:

| Role | Primary Collaborators | Key Touchpoints |
|------|----------------------|----------------|
| **Developer** | Product Owner, QA Lead, Scrum Master | Daily standups, PR reviews, backlog refinement |
| **Product Manager** | Product Owner, Stakeholders, Project Manager | Weekly alignment, roadmap reviews, prioritization |
| **Project Manager** | All roles | Status updates, risk reviews, coordination meetings |
| **Product Owner** | Developers, Scrum Master, Stakeholders | Backlog refinement, sprint planning, acceptance |
| **Scrum Master** | Developers, Product Owner, Project Manager | Agile ceremonies, impediment removal, process improvement |
| **Stakeholder Representative** | Product Owner, Product Manager, Project Manager | Reviews, feedback sessions, acceptance testing |
| **Release Manager** | Developers, QA Lead, Project Manager | Release planning, readiness reviews, deployments |
| **QA Lead** | Developers, Product Owner, Release Manager | Test planning, acceptance testing, quality gates |

