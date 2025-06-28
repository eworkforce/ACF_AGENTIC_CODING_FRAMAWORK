# ACF_AGENTIC_CODING_FRAMAWORK
Exhaustive Agentic Coding Framework

# ACF_AGENTIC_CODING_FRAMAWORK
Exhaustive Agentic Coding Framework

This  Framework encapsulates in a attempt to be exhaustive, a complete MECE ( Mutualy Exclusive   Collectivelly Exhaustive) approach to master AI  assited coding discipline with a systematic and methodic process flow.
It is structure aroung 6 mains   phases:
	1: INITIALISATION: Brief description of project  main goal and objective , Uses case, target users,  context
	2: REQUIREMENTS: Based on Initiatialisation , Create PRD ( project Requirements Description ) 
	3: ARCHITECTURE: Based on PRD, Create project technical Architecture including 
		-choice of Software descign architecture type (  VSA, layered Ach, Atomic arch, Mixted , Etc..), 
		-Technical Stack for Front end , back end.
	4: CONTEXT MANAGEMENT: Gathering of Specific resources involved in  PRD & ARCHI, includind:
		- Context resources
		- Tech Stack Document
		- MCP Implementation
	5: PRINCIPLES & RULES: Create  AI Guiderails Rule and  DEV  Principle aligned with   PDR & ARCHI
	6: WORKFOLOW & TASK MANAGEMENT: Implement  project Dev Workflow and task management tool and MCPs

# ACF to BMAD METHOD Mapping

This document provides a structured mapping of the Agentic Coding Framework (ACF) phases to the concepts, agents, and deliverables within the BMAD METHOD framework.

## 1: INITIALISATION
- **Required inputs/Document:** User's initial idea and project goals. Can also include existing market research or competitive analysis documents.
- **Deliverable outputs/Documents:** `project-brief.md`, `market-research.md`, or `competitor-analysis.md`.
- **BMAD Phase:** Planning Phase (Initial Step).
- **BMAD core Agents:** `analyst`.
- **BMAD Specialized Agents:** `analyst`.
- **Comments:** This phase directly corresponds to the `analyst` agent's role of performing initial research and creating a `project-brief.md` document, which serves as the foundation for the entire project.

## 2: REQUIREMENTS
- **Required inputs/Document:** `project-brief.md`.
- **Deliverable outputs/Documents:** `prd.md` (using `prd-tmpl`) or `brownfield-prd.md` (using `brownfield-prd-tmpl`).
- **BMAD Phase:** Planning Phase (PRD Creation).
- **BMAD core Agents:** `pm` (Product Manager).
- **BMAD Specialized Agents:** `pm` (Product Manager).
- **Comments:** The `pm` agent takes the `project-brief.md` as input to create the comprehensive Product Requirements Document (PRD).

## 3: ARCHITECTURE
- **Required inputs/Document:** `prd.md` (or `brownfield-prd.md`) and, for UI projects, `front-end-spec.md`.
- **Deliverable outputs/Documents:** A main architecture document (e.g., `architecture.md`, `fullstack-architecture.md`) and, if applicable, a `front-end-spec.md`.
- **BMAD Phase:** Planning Phase (Architecture Design).
- **BMAD core Agents:** `architect`, `ux-expert`.
- **BMAD Specialized Agents:** `architect`, `ux-expert`.
- **Comments:** The `architect` creates the technical architecture based on the PRD. For UI projects, the `ux-expert` first creates a `front-end-spec.md` which informs the architecture.

## 4: CONTEXT MANAGEMENT
- **Required inputs/Document:** The final, completed PRD and Architecture documents.
- **Deliverable outputs/Documents:** Sharded document folders (e.g., `docs/prd/`, `docs/architecture/`) created by the `shard-doc` task. The `bmad-core/core-config.yml` file is also a key artifact for managing context.
- **BMAD Phase:** Transition from Planning to IDE Development.
- **BMAD core Agents:** `po` (Product Owner), `sm` (Scrum Master).
- **BMAD Specialized Agents:** `po` (Product Owner), `sm` (Scrum Master).
- **Comments:** BMAD formalizes this step by sharding the main planning documents into smaller, manageable chunks that are used during the development cycle.

## 5: PRINCIPLES & RULES
- **Required inputs/Document:** The `prd.md` and the architect's analysis of the project requirements.
- **Deliverable outputs/Documents:** This is not a separate document but rather key sections within the main architecture document, such as "Coding Standards," "Test Strategy and Standards," and "Security."
- **BMAD Phase:** Planning Phase (embedded within Architecture).
- **BMAD core Agents:** `architect`.
- **BMAD Specialized Agents:** `architect`.
- **Comments:** The `architect` agent embeds these mandatory rules and standards directly into the architecture document, which then becomes the guide for the `dev` agent.

## 6: WORKFLOW & TASK MANAGEMENT
- **Required inputs/Document:** The sharded PRD and Architecture documents.
- **Deliverable outputs/Documents:** Sequentially created `story-X.X.md` files and, most importantly, the implemented code with passing tests.
- **BMAD Phase:** IDE Development Workflow.
- **BMAD core Agents:** `sm` (Scrum Master), `dev` (Developer), `qa` (QA Specialist).
- **BMAD Specialized Agents:** `sm`, `dev`, `qa`.
- **Comments:** BMAD implements this with a highly structured, sequential development loop where the `sm` agent creates a story, the `dev` agent implements it, and the `qa` agent reviews it.
