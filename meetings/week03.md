### Project Direction

Current Project Focus:
- Investigate how established software engineering practices should be applied when agentic AI performs a substantial portion of implementation.
- Particular focus on:
    - Agent autonomy and delegation of responsibilities
    - Guardrails and restrictions on agent behaviour
    - Human oversight throughout the SDLC
    - How AI-generated code should be reviewed, approved and integrated
- Consider how pull requests, code reviews and human approval can be incorporated into a structured development workflow.
### Progress Since Week 2
- Initial problem statement drafted.
- Five literature sources annotated:
    - SWEBOK Guide v4.0
    - Large Language Models for Software Engineering: A Systematic Literature Review
    - SWE-bench
    - SWE-agent
    - Human-in-the-Loop Software Development Agents
- Progress committed to GitHub
- Project scope remains broad and needs further refinement.
- More research needed into practical guardrails, pull-request workflows and code review.
### Aim and Objectives
Current working aim:
- Investigate how established software engineering practices should be applied when agentic AI performs a substantial proportion of software implementation.
Potential objectives:
- Review established SWE practices and agentic AI literature.
- Identify areas where human oversight and guardrails are required.
- Define a structured development workflow for an AI agent.
- Apply the workflow to a practical software project.
- Empirically evaluate different approaches.
- Compare the results against established SWE practices.

Objectives should be SMART: Specific, Measurable, Achievable, Relevant and Time-bound.
Distinguish between project objectives and software requirements:
- **Objectives:** What the overall research project aims to achieve.
- **Functional requirements:** What the practical software system must do.
- **Non-functional requirements:** Qualities and constraints such as security, performance and maintainability.

### Practical Use Case (Term 2)
The practical use case has not yet been finalised.
Two potential applications:
- **GitLock:** A version-control-inspired web application for managing Deadlock character builds.
- **LearnLock:** A personal improvement and match-review application for Deadlock players.

GitLock is currently the preferred option.
- Uses familiar software engineering concepts such as version control, branching and change tracking.
- Provides clear functional requirements and measurable acceptance criteria.
- Should be sufficiently complex to demonstrate meaningful software engineering decisions.
- Ideally, the application should have a distinctive problem domain while remaining practical to implement and evaluate.
- Suitability of the use case still needs to be confirmed.
### GitLock Requirements
Potential functional requirements:
- Users can register and log in.
- Users can create, save and manage Deadlock builds containing heroes, items, item progression, descriptions and patch versions.
- Users can create new versions of builds without overwriting previous versions.
- Users can view revision histories and changelogs.
- Users can fork existing builds to develop their own versions.
- Builds can be associated with specific game patches.
- Builds affected by changes to heroes or items can be flagged as potentially outdated.
- Users can search and filter builds by hero, patch, author or popularity.
- Builds can be made public or private.
- Users can follow or favourite builds and receive update notifications.

Additional features to consider:
- Visual version trees showing forks and development history.
- Comparisons between different versions of a build.
- Explanations or rationale for individual changes.
- Explicit patch compatibility rather than automatically treating builds as current.

Potential non-functional requirements
- Build history must be preserved without previous versions being overwritten.
- Changes must be traceable to a user and timestamp.
- Users must not be able to modify another user's build directly.
- Authentication and user data must be handled securely.
- The application should support concurrent users and reasonable response times.
- The codebase should be maintainable and modular.
- Patch data should be importable without requiring substantial changes to the application.
### Project Deliverables
- **Literature review** covering:
    - Established software engineering practices
    - Agentic AI in software development
    - Human oversight and guardrails
    - Methods for evaluating AI-assisted software engineering
- **Defined agentic development workflow** documenting:
    - Responsibilities delegated to the agent
    - Restrictions and guardrails
    - Stages requiring human approval
    - Code review and pull-request procedures
- **Practical software system** developed using the proposed workflow.
- **Empirical evaluation** comparing different agentic development approaches.
### Evaluation Criteria
Evaluation should focus on measurable outcomes directly related to the project's objectives.
Potential criteria
- **Task completion:** Whether the agent successfully completes assigned development tasks.
- **Functional correctness:** Whether implemented features meet requirements and pass tests.
- **Process adherence:** Whether the agent follows the defined development workflow.
- **Human intervention:** Frequency and stages at which human involvement is required.
- **Guardrail effectiveness:** Whether restrictions prevent undesirable actions or decisions.
- **Code and design quality:** Whether implementation aligns with established SWE practices.
- **Efficiency:** Time taken and human effort required.
Potentially compare different levels of agent autonomy, human oversight and guardrails to investigate their effect on development outcomes.
### Additional Considerations
- Consider appropriate backup arrangements, including cloud and external backups.
- Ensure bibliography entries include authors, publication dates and publication venues.
### Actions Before Week 4
- Finalise the project aim and objectives.
- Produce an outline of the expected project deliverables.
- Extend the literature review with five additional references.
- Continue developing the practical use case and initial requirements.
- Commit progress to the GitHub repository.