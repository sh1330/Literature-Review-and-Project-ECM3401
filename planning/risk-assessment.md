# Project Risk Assessment
### Project Management
#### R01 - Scope Creep
Risk: The research or practical application becomes too complex, exceeding the available time and resources.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Define clear project objectives and boundaries.
- Prioritise essential functionality and distinguish it from optional features.
- Review the project scope against milestones and available time.
##### Contingency:
- Remove or defer optional functionality.
- Reduce the scope of the practical application while preserving the requirements necessary for meaningful experimental evaluation.
#### R02 - Schedule Delays
Risk: Literature review, implementation or other development tasks take longer than expected, affecting subsequent milestones and submission deadlines.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Develop a realistic Gantt chart with milestones, dependencies and contingency time.
- Monitor progress against planned deadlines.
- Prioritise activities on the critical path.
- Account for competing university deadlines.
##### Contingency:
- Reallocate time from lower-priority tasks.
- Adjust dependent activities and reduce non-essential work.
- Prioritise completion of assessed deliverables and the research objectives.
- Requirements and Implementation
#### R03 - Technical Complexity
Risk: Database design, booking availability, concurrent reservations or other system requirements prove more difficult to implement than anticipated.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Develop clear requirements and an initial system architecture before implementation.
- Investigate appropriate database technologies and data models.
- Prototype complex functionality, particularly booking availability and prevention of conflicting reservations.
- Establish automated tests for critical functionality.
##### Contingency:
- Simplify non-essential system functionality.
- Reconsider architectural decisions where necessary.
- Prioritise a working implementation of essential booking functionality over advanced features.

#### R04 - Incorrect AI-Generated Code
Risk: AI agents produce implementations containing defects, security vulnerabilities or functionality that does not correctly satisfy the specified requirements.
##### Likelihood: High
##### Impact: High
##### Mitigation:
- Establish clear requirements and measurable acceptance criteria.
- Incorporate automated testing and human code review into the development workflow.
- Require testing and approval before integrating generated changes.
- Evaluate code against established software engineering practices.
##### Contingency:
- Reject or revert incorrect implementations.
- Provide corrective feedback and allow the agent to revise its implementation.
- Manually correct critical defects where necessary, recording interventions as part of the experimental evaluation.
#### R05 - Unintended Agent Behaviour
Risk: AI agents modify unauthorised files, make inappropriate design decisions or fail to follow the prescribed development workflow.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Define agent permissions, responsibilities and restrictions.
- Use isolated development environments and version control.
- Introduce human approval checkpoints for significant changes.
- Record agent actions to evaluate compliance with the workflow.
##### Contingency:
- Stop the agent's execution and review its actions.
- Restore affected files or configurations using version control or backups.
- Adjust agent permissions or guardrails before resuming development.
#### R06 - Model Availability and Technical Limitations
Risk: API downtime, context-window limitations or token exhaustion interrupt development tasks or experiments.
##### Likelihood: Medium
##### Impact: Medium
##### Mitigation:
- Investigate model limitations and available usage quotas before experimentation.
- Monitor token consumption and maintain concise task contexts.
- Save intermediate progress and agent logs.
- Identify alternative models or providers where practical.
##### Contingency:
- Resume experiments when services become available.
- Restore the last recorded development state following interruptions.
- Use an alternative model if necessary, documenting the change and its implications for experimental comparability.
#### R07 - Excessive Costs
Risk: Model usage, repeated experiments or infrastructure costs exceed the available project budget.
##### Likelihood: Medium
##### Impact: Medium
##### Mitigation:
- Investigate cost-effective models and agent frameworks.
- Estimate costs and establish usage limits before conducting experiments.
- Monitor token consumption and API expenditure.
- Conduct small-scale pilot experiments before committing resources to full evaluations.
##### Contingency:
- Reduce unnecessary agent iterations and repeated executions.
- Consider lower-cost or locally hosted models where feasible.
- Adjust the number of experimental repetitions while acknowledging the impact on the reliability of the results.
- Research and Evaluation
#### R08 - Experimental Validity
Risk: Inconsistent experimental conditions, insufficient data or uncontrolled variables make results difficult to interpret, reproduce or compare.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Define experimental variables, controlled conditions and evaluation criteria before experimentation.
- Use consistent development tasks, model configurations and testing procedures.
- Record agent actions, outcomes and human interventions.
- Conduct pilot experiments to identify methodological weaknesses.
##### Contingency:
- Revise the experimental procedure before conducting the main evaluation.
- Repeat invalid or inconsistent experiments where possible.
- Document limitations and avoid drawing conclusions unsupported by the collected evidence.
#### R09 - Insufficient Evaluation Time
Risk: Implementation takes longer than expected, leaving insufficient time to conduct experiments, analyse results and complete the final report.
##### Likelihood: Medium
##### Impact: High
##### Mitigation:
- Allocate dedicated time for experimentation and analysis within the project schedule.
- Develop the evaluation methodology alongside the practical application.
- Prioritise development tasks that are necessary for the experimental investigation.
- Begin pilot experiments as early as practical.
##### Contingency:
- Reduce non-essential application functionality.
- Narrow the experimental scope to a smaller but controlled comparison.
- Prioritise obtaining meaningful results and completing the critical analysis over additional implementation features.