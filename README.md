# team-health

This is a list of measures that I have used in the past for how well a software development team is following best practices. A lot of these measures are subjective, and that's ok for these purposes. The goal was to track progress month-to-month, but the main benefit here is to force you to think about these measures and evaluate the team.

I used to have this in a spreadsheet format, and I'll try to add one of those in the near future.

Feel free to contribute suggestions!

## Team Health

**Team Cohesion**: We have the mutual trust and respect necessary to be an effective team for healthy collaboration. We have a strong sense of connectedness between members.

**Cross-Functional**: We have the right people, with the right skills, in the right clearly-defined roles. This enables us to successfully deliver the value for which this team is accountable.

**Encouraging Difference**: We seek and voice different viewpoints from diverse sources, both internally and externally, and we take the time to respectfully work through points of differences.

**Shared Understanding**: We share an understanding of our mission and purpose and our key milestones to deliver our strategic plan effectively as a team.

**Value and Metrics**: We understand the value we provide and the value back to the business, our definition of success and how that value is tracked and measured. We ultimately leverage our metrics to make decisions and action as necessary.

**Suitable Ways of Working**: Our ways of working together within the team enable us to do our jobs effectively, whether we are distributed or co-located. This includes the tools we use, how we meet and collaborate, and how we make decisions.

**Engagement and Support**: It's clear to other teams how and when to engage with us, teams do this effectively and consistently receive the support they need to progress. We have a clear understanding of who we depend on, and who depends on us.

**Continuous Improvement**: We always make time to celebrate our successes as well as earnestly reflect on, take action against, and fulfill our improvement opportunities. We have regular and intentional feedback loops within and outside of the team to make improvement decisions.

## Automated Testing

**Lint**: We automatically check our code with linting tools such as PyLint, shellcheck, or eslint to ensure a consistent coding style.

**Unit Tests**: We test small units of code are in isolation, using mocks for external dependencies.

**Integration Tests**: We test our application's integrations with external dependencies (databases, APIs, etc.) to ensure proper action of each with a variety of inputs.

**End-to-End Tests**: We automatically test our application as if by an end user, using tools such as Selenium, Cypress, Postman, etc.

**Accessibility Tests**: We automatically scan the frontend for accessibility violations. (But see also the manual testing under "Delivery")

**Coverage**: Our tests are comprehensive and meaningfully cover application code (90%+), integrations, and features. We do not comment out tests when they fail.

## Infrastructure as Code

**Version Control**: We use an Infrastructure-as-Code tool such as Terraform or CloudFormation to maintain all of our infrastructure in version control.

**Secrets**: Secrets are never stored within version control; we use appropriate methods to query them from secure stores like AWS Secrets Manager.

**Idempotent**: Re-deploying the same infrastructure configuration will yield the same result.

**Immutable**: We deploy a new instance rather than modifying an existing one.

## Continuous Integration / Continuous Delivery

**Code Quality**: We use branches, pull/merge requests, and meaningful code reviews to ensure that everything merged into the main branch is of high quality.

**Continuous Integration**: We integrate all work into the main branch once completed, and we do not have long-lived feature branches.

**Single-Step Deployment**: We can build and deploy our application in a single step (plus perhaps a manual confirmation step).

**Required Tests**: Our CI/CD pipelines require all automated tests to pass before a deployment.

**Continuous Delivery**: We make frequent deployments to production.

**Lower Environments**: We use separate environments for testing and production.

**Rollback**: We can roll back using the same or simpler process than deployment.

## Monitoring and Observability

**Service-Level Indicators**: We have defined our SLIs in conjunction with the client, and they align with the application's objectives.

**Metrics**: We collect meaningful metrics, informed by the SLIs, and we use Dashboards to quickly indicate system health.

**Logging**: We collect structured logs in a central location, and they include relevant metadata.

**Alerts**: We have alerts to notify us of problems or anomalies, and they go somewhere that we will see quickly.

**Traces**: We use distributed traces for troubleshooting and performance analysis.

**Reliability Testing**: We periodically test the performance, scaling, and reliability of our application to ensure that it will work properly during peak usage periods.

## Security and Compliance

**Access Control**: We have strong access control mechanisms, including least privilege principles, role-based access control, and multi-factor authentication.

**Incidents**: We have established incident management processes and workflows that include plans for notifying users and escalation to appropriate personnel.

**Encryption**: We encrypt our data at rest and in transit.

**Backups**: We regularly back up our data, and we periodically test data restoration processes.

**Static Analysis**: Our automated testing includes static security analysis of application code, dependencies, container images, and infrastructure using tools like SonarQube, trivy, or Docker Scout.

**Application Scans**: Our automated testing includes security scans (such as OWASP's ZAP) of web applications and APIs.

**Remediation**: We have established clear expectations regarding the timeliness of remediating security vulnerabilities, and we achieve or surpass those timelines.

**Compliance**: In conjunction with the client, we have identified compliance requirements and thoroughly documented our compliance efforts.

## Delivery

**Iterative Development**: We build our systems iteratively, make regular releases, and incorporate user feedback into future work.

**Feature Generation**: Our team is actively involved in the process to understand user needs. The team helps clients create features that meet user needs while also being feasible in terms of time and technical constraints.

**Ownership**: Our team owns and participates in all steps of delivery, from feature generation to release.

**Forward-Looking**: We architect our code and systems for extensibility and resilience to change.

**Accessibility**: We regularly perform thorough manual testing of frontend systems for accessibility using assistive devices. We meet all relevant Web Content Accessibility Guidelines (WCAG) standards.

**Documentation**: We maintain appropriate documentation for existing code and systems for all audiences (future developers on the project, any other team that integrates with the system, etc.). We store documentation as close to the application code as possible, preferably in version control.

**Technical Debt**: We continuously address tech debt, ensuring that at least some of each sprint goes to improve the code, infrastructure, documentation, or developer experience.

**Progress**: In this time period, we have made visible progress on our highest priorities.
