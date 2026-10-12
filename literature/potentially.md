#### Guide to the Software Engineering Body of Knowledge (SWEBOK Guide), Version 4.0
- **Editor:** Hironori Washizaki
- **Released:** 15 October 2024

https://www.computer.org/education/bodies-of-knowledge/software-engineering

To be used as the guide for what counts as "good" practices and design choices

#### Large Language Models for Software Engineering: A Systematic Literature Review
- **Authors:** Xinyi Hou, Yanjie Zhao, Yue Liu, Zhou Yang, Kailong Wang, Li Li, Xiapu Luo, David Lo, John Grundy, Haoyu Wang
- **Released:** 21 August 2023

https://arxiv.org/pdf/2308.10620

Literature review on ~400 studies and categorises use across six software engineering areas, including requirements engineering, design, development, quality assurance, maintenance and management.

Will also be good for snowball referencing

#### SWE-bench: Can Language Models Resolve Real-World GitHub Issues?
- **Authors:** Carlos E. Jimenez, John Yang, Alexander Wettig, Shunyu Yao, Kexin Pei, Ofir Press, Karthik Narasimhan
- **Released:** 10 October 2023

https://proceedings.iclr.cc/paper_files/paper/2024/file/edac78c3e300629acfe6cbe9ca88fb84-Paper-Conference.pdf

Use this for evaluating how a model is tested; looking at how they benchmarked the models. measuring success.

#### SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering
- **Authors:** John Yang, Carlos E. Jimenez, Alexander Wettig, Kilian Lieret, Shunyu Yao, Karthik Narasimhan, Ofir Press
- **Released:** 6 May 2024

https://proceedings.neurips.cc/paper_files/paper/2024/file/5a7c947568c1b1328ccc5230172e1e7c-Paper-Conference.pdf

For the 'guardrails', they tested what tools and environments you should provide to an agent to influence its behaviour and effectiveness given a problem

#### Human-In-the-Loop Software Development Agents

**Authors:** Wannita Takerngsaksiri, Jirat Pasuksmit, Patanamon Thongtanunam, Chakkrit Tantithamthavorn, Ruixiong Zhang, Fan Jiang, Jing Li, Evan Cook, Kun Chen, Ming Wu

Released: 19 November 2024

https://arxiv.org/pdf/2411.12924

This paper introduces HULA, a human-in-the-loop framework that allows developers to review and approve AI-generated coding plans and code changes. The researchers evaluated the framework at Atlassian, finding that 82% of generated plans were approved, 25% of code-generated issues resulted in pull requests, and 59% of those pull requests were merged. This will be useful for investigating how human oversight can be integrated into agentic software development, particularly when deciding where approval checkpoints and code reviews should be required in my project's development workflow.

#### MetaGPT: Meta Programming for a Multi-Agent Collaborative Framework
- **Authors:** Sirui Hong, Mingchen Zhuge, Jonathan Chen, Xiawu Zheng, Yuheng Cheng, Ceyao Zhang, Jinlin Wang, Zili Wang, Steven Ka Shing Yau, Zijuan Lin, Liyang Zhou, Chenyu Ran, Lingfeng Xiao, Chenglin Wu
- **Released:** 1 August 2023

https://arxiv.org/pdf/2308.00352
This paper introduces MetaGPT, a multi-agent framework that uses predefined roles and Standard Operating Procedures (SOPs) to structure software development tasks. It demonstrates how established software engineering practices can improve coordination between AI agents. This will be useful for defining a structured development workflow in my project, particularly how predefined processes and responsibilities can guide agent behaviour.

#### Benchmarking and Studying the LLM-based Agent System in End-to-End Software Development
- **Authors:** Zhengran Zeng, Yixin Li, Rui Xie, Wei Ye, Shikun Zhang
- **Released:** 6 November 2025

https://arxiv.org/pdf/2511.04064

This paper investigates how different agent architectures and development workflows affect performance in end-to-end software development. The researchers compared three agent configurations using a controlled experimental setup, evaluating functional correctness and requirements satisfaction. This will be useful for designing fair and repeatable experiments in my project, particularly when defining evaluation criteria, controlling variables and measuring how effectively agents meet software requirements.

#### AgentSpec: Customizable Runtime Enforcement for Safe and Reliable LLM Agents
- **Authors:** Haoyu Wang, Christopher M. Poskitt, Jun Sun
- **Released:** 24 March 2025

https://arxiv.org/pdf/2503.18666

This paper introduces AgentSpec, a framework that allows developers to define and enforce rules on what an AI agent can do while running. It uses predefined constraints to prevent unsafe actions, rather than relying solely on instructions given to the agent. The researchers tested this across several domains, including code execution, where it prevented over 90% of unsafe executions. This will be useful for investigating how guardrails can actually be implemented and enforced in my project, particularly when controlling what actions an agent is allowed to perform during software development.

#### Automated Code Review in Practice
- **Authors:** Umut Cihan, Vahid Haratian, Arda İçöz, Mert Kaan Gül, Ömercan Devran, Emircan Furkan Bayendur, Baykal Mehmet Uçar, Eray Tüzün
- **Released:** 24 December 2024

https://arxiv.org/pdf/2412.18531

This paper investigates the use of LLM-based automated code review tools in real software development environments. The researchers analysed 4,335 pull requests, with 1,568 receiving automated reviews. They found that 73.8% of automated review comments were resolved, but pull requests took longer to complete, and some reviews contained incorrect or unnecessary feedback. This will be useful for investigating how AI-generated code should be reviewed and approved, and whether automated code review can improve code quality. It could also help inform the pull request and human oversight processes used in my project.

#### Exploring the Use of LLMs for Requirements Specification in an IT Consulting Company
- **Authors:** Liliana Pasquale, Azzurra Ragone, Emanuele Piemontese, Armin Amiri Darban
- **Released:** 25 July 2025

https://arxiv.org/pdf/2507.19113
This paper investigates how LLMs can be used to generate software requirements specifications and user stories from existing documentation in a real IT consulting company. The researchers compared requirements generated by three LLMs against those produced by human analysts. They found that LLMs could reduce the time and effort required, but the quality of the generated requirements depended heavily on the information provided and often required human revision. This will be useful for investigating which parts of requirements engineering can be delegated to an AI agent and where human oversight is needed, particularly when defining requirements and approval stages within my development workflow.