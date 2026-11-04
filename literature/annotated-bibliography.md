#### Guide to the Software Engineering Body of Knowledge (SWEBOK Guide), Version 4.0
**Washizaki, H. (editor) - IEEE Computer Society**
https://www.computer.org/education/bodies-of-knowledge/software-engineering?utm_source=chatgpt.com#about
SWEBOK will provide a general overview of accepted practices within SWE. It covers software requirements, architecture and design, testing, engineering process and SWE management. For this project SWEBOK provides a baseline for SWE practices and will be used as a basis for assessing an agentic AI system. It will be used to determine if the AI agent follows appropriate practices during the SDLC.
A limitation for this source is that it is very general and broad, and is not specifically concerned with agentic AI. More recent literature will be required to investigate how practices may need to change when AI agents are involved.

#### Hou, X. et al. - Large Language Models for Software Engineering: A Systematic Literature Review
https://arxiv.org/pdf/2308.10620
This paper is a systematic literature review of 395 studies published between 2017 and 2024, looking at how large language models have been applied within software engineering. The review considers the types of models used, how datasets are collected and prepared, how model performance is optimised and evaluated, and which software engineering tasks have seen successful applications.
For this project, the paper is useful because it provides a broad overview of LLM use across software engineering and helps review which parts of the SDLC have already been studied. It will also be used for snowball referencing to identify more specialised literature.
A limitation for this source is that it focuses on LLMs in SWE generally, rather than specifically on agentic SWE systems, therefore more specialised literature is needed for questions around autonomy, guardrails, and human oversight.

#### Jimenez, C. E. et al. - SWE-bench: Can Language Models Resolve Real-World GitHub Issues?
https://proceedings.iclr.cc/paper_files/paper/2024/file/edac78c3e300629acfe6cbe9ca88fb84-Paper-Conference.pdf
This paper introduces SWE-bench, a benchmark for evaluating large language models on real world software issues collected from GitHub. Given a codebase and an issue, a language model is tasked with generating a patch that resolves the described problem. The proposed changes are then evaluated by running tests to determine whether the issue has been fixed without breaking existing features
For this project, this paper will be used as an example on how SWE performance can be evaluated in a measurable way. The use of executable tests is relevant when looking at how the performance of an agentic AI system could be assessed during the practical part of the project
A limitation for this source is that SWE-bench mainly evaluates the final code change successfully resolving an issue, it doesn't evaluate whether or not the model followed good SWE practices.

#### Yang, J. et al. - SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering
https://proceedings.neurips.cc/paper_files/paper/2024/file/5a7c947568c1b1328ccc5230172e1e7c-Paper-Conference.pdf
This paper introduces SWE-agent, a system that allows a language model to interact with a repository through an Agent-Computer Interface (ACI). The agent can perform tasks such as searching files, viewing code, editing files and running tests. The paper looks at how the design of these tools and the feedback given to the agent can affect its ability to complete SWE tasks.
This paper will be useful because it shows us that the performance of an agentic AI system depends on the environment, tools and constraints provided to it. This will be relevant to the projects research on guardrails.
A limitation for this paper is that it focuses on repository level implementation and bug fixing tasks. It doesn't say much about how agentic AI should be managed across the wider stages of the SDLC, such as requirements or design.

#### Takerngsaksiri, W., Pasuksmit, J., Thongtanunam, P., Tantithamthavorn, C., Zhang, R., Jiang, F., Li, J., Cook, E., Chen, K. & Wu, M. - Human-In-the-Loop Software Development Agents
https://ieeexplore.ieee.org/document/11121706 - access with institutional sign in
This paper introduces HULA, a human in the loop software development agent framework designed to support developers. HULA divides work between an AI Planner Agent, an AI Coding agent, and a human developer. The human can review and modify the generated plan , approve it before coding begins, review generated code and decide whether a pull request should be raised.
The framework was deployed internally at Atlassian and evaluated using SWE-bench and real tasks. In practice, 82% of generated plans were approved by developers, but only 25% of generated code changes were raised as pull requests. Developers also reported that the generated code was generally easy to modify and understand , but concerns around incorrect or incomplete code were raised. For this project, HULA is going to be relevant when investigating human oversight and guardrails.
A limitation on this paper is that the study was based around Atlassian's internal development environment and relies on GPT-4, therefore their findings may not generalise to other models or other environments.

#### Hong, S. et al. - MetaGPT: Meta Programming for a Multi-Agent Collaborative Framework
https://arxiv.org/pdf/2308.00352
This paper introduces MetaGPT, a multi-agent framework that uses predefined roles and Standard Operating Procedures (SOPs) to structure software development. Different agents are assigned roles such as project manager, architect and engineer, with each responsible for specific tasks. The researchers compared MetaGPT against other multi-agent systems and found that using structured processes helped improve coordination between agents and reduce errors.

For this project, MetaGPT will be useful when looking at how established SWE practices can be used to structure an agentic development workflow. It also provides an example of how assigning responsibilities and following predefined processes can influence agent behaviour.

A limitation for this paper is that it focuses mainly on communication and coordination between multiple AI agents, rather than how human developers should oversee their work. Therefore, more research is needed into human oversight and approval stages.

#### Zeng, Z. et al. - Benchmarking and Studying the LLM-based Agent System in End-to-End Software Development
https://arxiv.org/pdf/2511.04064
This paper investigates how different agent architectures and development workflows affect performance in end-to-end software development. The researchers developed E2EDevBench, a benchmark for evaluating agents on software development tasks, and compared three different agent configurations. They evaluated the agents using automated testing and requirements satisfaction, finding that agents satisfied around 50% of the requirements, with problems often caused by missing requirements and insufficient verification.

For this project, the paper will be useful when looking at how to design and conduct experiments comparing different agentic development approaches. It provides examples of how performance can be measured using functional correctness and requirements satisfaction, as well as how experimental conditions can be controlled.

A limitation for this paper is that it mainly compares agent architectures rather than investigating the effects of human oversight and guardrails. It also uses LLMs to evaluate some requirements, which may affect the reliability of the results.

#### Wang, H., Poskitt, C. M. and Sun, J. - AgentSpec: Customizable Runtime Enforcement for Safe and Reliable LLM Agents
https://arxiv.org/pdf/2503.18666
This paper introduces AgentSpec, a framework that allows developers to define and enforce restrictions on what AI agents can do during execution. Rather than relying only on instructions given to the agent, AgentSpec uses predefined rules to monitor and prevent certain actions. The researchers tested the framework across different environments, including code execution, and found that it prevented over 90% of unsafe executions in the code-agent tests.

For this project, AgentSpec will be useful when investigating how guardrails can be implemented and enforced within an agentic development workflow. It shows how restrictions can be actively enforced rather than simply relying on an agent to follow instructions.

A limitation for this paper is that it mainly focuses on preventing unsafe agent actions, rather than whether the agent follows good SWE practices or produces high-quality code. Therefore, other methods would be needed to evaluate the quality of the development process.

#### Cihan, U. et al. - Automated Code Review in Practice
https://arxiv.org/pdf/2412.18531
This paper investigates the use of LLM-based automated code review in a real software development environment. The researchers analysed 4,335 pull requests across three projects, with 1,568 receiving automated reviews. They found that 73.8% of automated review comments were resolved, but pull requests generally took longer to complete. The automated reviews also sometimes produced incorrect or unnecessary feedback.

For this project, the paper will be useful when investigating how AI-generated code should be reviewed and approved before being integrated into a project. It also shows some of the potential benefits and problems with automated code review, which could help when deciding where human review and approval should be required in the development workflow.

A limitation for this paper is that it focuses on automated code review within a particular development environment, so the results may not apply to other projects. Also, resolving review comments does not necessarily mean that the resulting code is correct or of better quality.

#### Pasquale, L. et al. - Exploring the Use of LLMs for Requirements Specification in an IT Consulting Company
https://arxiv.org/pdf/2507.19113
This paper investigates how LLMs can be used to generate software requirements specifications and user stories from existing documentation in an IT consulting company. The researchers compared requirements produced by three LLMs against those written by human analysts. They found that LLMs could reduce the time and effort required to produce requirements documents, but the quality of the results depended on the information provided and often required human revision.

For this project, the paper will be useful when investigating which parts of requirements engineering can be delegated to an AI agent and which should remain human-led. It will also help when deciding how requirements should be reviewed and approved before implementation begins.

A limitation for this paper is that it focuses on generating requirements from information that has already been collected, rather than the whole requirements engineering process. The study was also carried out within a single company, so the results may not generalise to other development environments.