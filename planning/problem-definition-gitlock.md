Version-Controlled Deadlock builds
### Background
##### What is Deadlock?
- Deadlock is a highly competitive 6vs6 multiplayer game developed by Valve, combining elements of multiplayer online battle arenas (MOBAs) with third person shooters, such as League of Legends and Overwatch. Deadlock has a large player base with it recently surpassing 250,000 concurrent players, whilst still being in a invitation only closed-beta.
- Players select characters, known as heroes, each with unique abilities and playstyles. During matches, players earn in game currency called souls, which can be spent on items, of which there are 156 unique items, that can improve their hero's capabilities
- Items can be divided into three main categories:
	- Spirit: Enhance abilities and their effects
	- Vitality: Improve health, survivability and mobility
	- Weapon: Improves weapon damage and combat effectiveness
- The selection and progression of items play a significant role in a hero's effectiveness, making strategic item planning and management an essential part of the game.
- A game of Deadlock is ~30-40 minutes, where the outcome of a match is essentially decided on who has the better item economy and team play.
##### What is a Build?
A build is a planned configuration of items and ability upgrades for a particular hero, designed to achieve a specific playstyle or strategic objective.
- Build typically include:
	- Recommended items and their purchase order
	- Ability upgrade priorities
	- Alternative items for different match situations
	- Explanations of particular choices
- Builds are a fundamental part of Deadlock's strategy, with players regulary creating, sharing and following builds created by pplayers.
- This has led to several dedicated platforms just for builds including:
	- Deadlocklabs.gg 
		- https://deadlocklabs.gg/builds/paige-spreading-kindness-yuri-s-support-paige-3-745893/
		- Example of a build ^, the design of the system would be similar to this example for the creation/editing of a build due to the in-game build creation/editing style looking like this, but this could change.
	- statlocker.gg
	- mobalytics.gg
- These services show an established ecosystem for creating, discovering and sharing builds
### The Problem
- Deadlock is currently in closed beta and remains under active development, receiving frequent updates that change hero abilities, item statistics and gameplay mechanics.
- Therefore, the game is in a volatile state where a previously effective build may become significantly weaker or even useless following a patch, alternatively changes to certain items or abilities may make a build considerably stronger
- Players therefore must continually reassess and adapt their builds to remain competitive
- While existing platforms support build creation and discovery, GitLock proposes a more structured approach to managing how builds evolve over time.
- The key problems it aims to address include:
	- Version History: Preserving previous build configurations rather than simply replacing them
	- Change Tracking: Recording what changed between revisions and why.
	- Forking: Allowing players to create independent variations of existing builds while preserving their origin
	- Patch Compatibility: Identifying builds potentially affected by game updates.
	- Traceability: Understanding how builds have evolved across different game versions
- This creates a practical need of a system that treats builds as evolving, version-controlled configurations rather than static collections of items
### Proposed Application - GitLock
- GitLock (Git(Hub Dead)lock 🤯) is a version-control-inspired web application that allows Deadlock players to create, manage, revise, compare, and fork character builds
- Drawing inspiration from software version-control systems such as Git, it would introduce structured change management to Deadlock builds, with community features that could include comments, forks, notes/explanations of choices etc.
#### Essential Functionality
- Create, view, edit, and delete builds
- Associate builds with heroes and items
- Save revisions and record changelogs
- View version histories and compare revisions
- Ability upgrade sequences, in what order should abilities be upgraded
- Item progression stages, early game, mid-game etc.
#### Core functionality
- Fork existing builds while preserving their original source
- Record game patches and flag builds affected by changes
- Visual version tree that will display the history of a build, including revisions, forks, similar to Git branches
- Restoration of previous versions, allowing authors to restore an older configuration by creating a new revision from it
#### Optional Functionality
- User comments and discussions
- Filtering or censoring inappropriate build names
- Branches, allowing users to maintain multiple variations of a build, such as defensive or aggressive configurations
- Change explanations, allowing authors to explain why particular items or abilities were changed
- Comparison of builds, allowing comparison of independently created builds
- Build release versions, allowing authors to mark revisions as recommended, experimental or stable.
- Merging, allowing users to incorporate selected changes from another fork or build
- Build pull requests
- Community proposed changes with reviews from authors
- Build tags
### Example use case
- A player creates and publishes a build for a particular hero. Another player discovers it but prefers a different item progression, so they fork the original build and modify it.
- Following a game update, an item used by both builds is changed. GitLock identifies the affected builds and flags them for review
- The original author updates their build, creating a new revision with a changelog. Other players can compare the revisions to understand what changed, while the previous version remains accessible
### Software Engineering Depth
- Although GitLock is a conventional web application, its functionality presents quite a few non-trivial engineering challenges
- ###### Requirements Engineering:
	- Identify stakeholders, including build creators, build consumers, community contributors, and application administrators
	- Capture different stakeholder needs and view points
	- Develop user stories, use cases, and measurable acceptance criteria
	- Validate requirements through perspectives beyond my own by reviewing the stakeholders, and their view points by utilising user stories, and use cases
- ###### System Design and Data Modelling
	- Design relationships between users, heroes, items , builds, revisions and patches (I especially think the storing of the items will be quite challenging due to there being a lot of different effects/abilities different items can have e.g. passive items, active items).
	- Preserve historical revisions while maintaining data integrity
	- Represent forks and their relationships to original builds
	- Determine how patch changes affect existing and historical configurations (This one might be particularly tricky due to how items interact with each other, for example a low tier item might get a small decrease in its stats but that small decrease significantly reduces its scalability later in the game)
- ###### Implementation and Testing
	- Implement authentication, authorisation, and build management
	- Develop revision comparison, forking and patch-impact detection
	- Handle edge cases involving deleted builds, historical versions and ownership
	- Test functional correct, security, and data integrity
- These challenges require meaningful architectural decisions, requirements analysis and testing beyond basic CRUD operations
### Relevance to the Research Project
GitLock would serve as the practical case study for investigating how established software engineering practices should be applied when agentic AI performs a substantial proportion of software implementation
- Its functionality provides development tasks of varying complexity, allowing the project to investigate:
	- Which software engineering activities can be delegated to an AI agent
	- How agent autonomy, guardrails and human oversight affect development
	- Whether agents follow established software engineering practices
	- How generated implementations can be reviewed, tested and evaluated
- The application would initially focus on its essential and core functionality, using predefined or manually recorded patch data to avoid unnecessary reliance on external integrations

The primary research focus remains on the development and empirical evaluation of the agentic software engineering workflow, with GitLock serving as the realistic and sufficiently complex application through which I would investigate it.
