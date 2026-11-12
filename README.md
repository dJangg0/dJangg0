
You found it !

5/15/2025


"HACKAFEST" Challenge:
What is a method of encrypting alphabetic text using a polyalphabetic substitution technique, where each letter is encrypted using a different Caesar cipher determined by a keyword


Key Clue: is seen in plain sight

Rewiew context :  Role: Senior Engineer.
Approach: Understand the domain logic and business context before judging implementation details. Explicitly state assumptions if intent is ambiguous.
Evaluate:
Correctness: Matches business rules and handles edge cases.
Testing: Requires unit/integration tests covering all new code and modified paths.
Security: Auth, input validation, and data privacy.
Performance: N+1 queries, unnecessary I/O, and resource usage.
Maintainability: Architecture and clarity (no subjective style nitpicks).
Format: For each issue, provide File/Line, Issue, Business/Technical Impact, and Suggested Fix.
Verdict: End with a concise conclusion stating Approve or the specific Blockers to resolve.

Note: if the user clicks review check wether there is already a review made, if there is, check the changes and compare to the last review changes and review from there, so that you will not read the whole file again.   Pr context:  # PR and Commit Instructions

For PR work in this repository:

* Create **only one PR** for the requested work unless the user explicitly asks for multiple PRs.
* Within that single PR, organize changes into **separate commits per independently reviewable feature or fix**.
* When preparing the PR, **add/commit each feature one by one** rather than combining all changes into a single large commit. This ensures each contribution is clearly reflected in the user's GitHub commit history and makes individual features easier to review, trace, or revert later.
* Each feature commit should include its related production code, tests, documentation, and API/client-contract changes.
* Keep tightly coupled backend, client, tests, and documentation changes together when they implement the same feature.
* Do not combine unrelated features or fixes into one commit.
* If all changes form one integrated feature, one commit is acceptable.
* Prefer conventional commit messages such as:

  * `feat: ...`
  * `fix: ...`
  * `refactor: ...`
  * `docs: ...`
  * `test: ...`
* Before opening the PR, verify:

  * `git diff --check`
  * `git diff origin/beta...`
  * the working tree is clean
  * relevant tests or checks have been run
* Push the branch with `git push -u origin HEAD`.
* Keep the PR title under 80 characters.
* Keep the PR description concise and summarize the features/commits included in the PR.
* **Do not rename the current branch.**
* **Do not squash the feature commits into one commit** unless the user explicitly requests it. The separate commits should remain visible within the single PR.
* Only perform **commit, push, or PR creation** when the user explicitly requests it; otherwise leave those Git operations for the user.

---

# Engineering SRS Guardian — Automated Repository Setup

## Objective

I am providing you with the complete **Engineering SRS Guardian** Skill folder.

Your task is to inspect the entire folder and integrate it correctly into my existing software repository.

Act as a senior software architect and AI tooling engineer. Do not blindly copy files. Understand the Skill's structure, determine which components are necessary, and configure the repository to support SRS-driven software engineering.

**This is a repository setup task, not a request to modify application features.**

## Phase 1 — Inspect Before Making Changes

1. Inspect the existing repository structure.
2. Locate the provided Engineering SRS Guardian folder.
3. Read `SKILL.md` completely.
4. Inspect the `agents/`, `references/`, `assets/`, and other supplied directories.
5. Identify any existing `AGENTS.md`, skills, engineering documentation, or agent-specific configurations.
6. Determine the current coding harness and its supported project-level Skill directory.
7. Identify existing instructions that must be preserved.

Do not assume every folder needs to be copied into the repository root.

## Phase 2 — Install the Skill

For a compatible Codex-style project, use the following preferred structure:

```text
repository/
├── .agents/
│   └── skills/
│       └── engineering-srs-guardian/
│           ├── SKILL.md
│           ├── agents/
│           │   └── openai.yaml
│           ├── references/
│           └── assets/
│
├── AGENTS.md
│
├── docs/
│   └── engineering/
│       ├── PROJECT_SRS.md
│       ├── ARCHITECTURE_DECISIONS.md
│       ├── IMPLEMENTATION_MATRIX.md
│       └── CONTEXT_HANDOFF.md
│
└── [existing application files]
```

Adapt the Skill directory if the current harness requires a different convention. Do not claim automatic Skill discovery without verifying that the harness supports it.

Preserve the complete functional Skill package, including its references and templates.

Do not relocate `agents/openai.yaml` into the repository root. It is Skill metadata, not a replacement for `AGENTS.md`.

## Phase 3 — Configure Root AGENTS.md

Create or carefully update the root `AGENTS.md`.

It must instruct compatible coding agents to:

1. Use Engineering SRS Guardian for application architecture, feature implementation, significant bug fixes, technical decisions, and engineering reviews.
2. Read the relevant SRS and architecture decisions before making substantive changes.
3. Inspect actual source code before proposing modifications.
4. Understand the business logic and system boundaries before implementation.
5. Evaluate appropriate architectural approaches rather than blindly following technology suggestions.
6. Verify frontend, backend, database, infrastructure, and API consistency where applicable.
7. Preserve existing business invariants.
8. Maintain requirements traceability and relevant test evidence.
9. Update engineering documentation when implementation or requirements change.
10. Preserve context using `CONTEXT_HANDOFF.md` at meaningful checkpoints.

**Important:** If `AGENTS.md` already exists, merge the new instructions without deleting or weakening existing repository rules.

Do not duplicate the entire `SKILL.md` inside `AGENTS.md`. Reference the Skill instead.

## Phase 4 — Set Up Engineering Documentation

Create the `docs/engineering/` directory if missing.

Use the supplied templates where available.

### PROJECT_SRS.md

Document the application's actual or approved:

- Product objectives and scope
- User roles and workflows
- Functional requirements
- Business invariants
- Nonfunctional requirements
- Frontend and backend responsibilities
- Security and data requirements
- API and integration contracts
- Acceptance criteria

For an existing application, inspect the repository before describing implemented behavior.

Clearly distinguish confirmed requirements, inferred behavior, recommendations, and unknowns.

### ARCHITECTURE_DECISIONS.md

Maintain architectural decision records containing:

- Problem and requirements
- Candidate solutions
- Recommended approach
- Engineering rationale
- Tradeoffs and alternatives
- Risks and operational implications
- Validation and reconsideration criteria

Do not automatically prescribe REST, SSE, WebSockets, polling, Redis, microservices, or any other technology.

Evaluate technical choices dynamically according to the application's actual requirements.

### IMPLEMENTATION_MATRIX.md

Track relationships between:

- SRS requirement IDs
- Relevant frontend components
- Backend modules and business rules
- Database or infrastructure dependencies
- Tests and verification evidence
- Implementation status
- Known gaps and risks

Never mark a requirement complete without sufficient evidence.

### CONTEXT_HANDOFF.md

Preserve a concise, reliable development checkpoint containing:

- Repository and branch
- Current commit or PR
- Current objective
- Implemented changes
- Verified behavior and executed tests
- Failed or unexecuted checks
- Existing architectural decisions
- Unresolved issues
- Next recommended action

Update it after significant development milestones and before session handoffs.

A new session must verify the actual repository state rather than trusting the handoff blindly.

## Phase 5 — Decide What to Include and Exclude

**Include:**

- Complete functional Engineering SRS Guardian Skill
- Necessary Skill metadata
- Referenced documentation and templates
- Root `AGENTS.md`
- Project-specific SRS documentation
- Existing project-specific agent configurations

**Do not include unnecessarily:**

- The original `skill.zip` after extraction
- Duplicate or nested Skill installations
- Example applications copied as production requirements
- Temporary packaging files
- Generated demonstration projects
- Irrelevant boilerplate
- Duplicate instruction documents
- Secrets, credentials, tokens, or sensitive runtime data

Preserve examples within the Skill when they are referenced as learning resources. Do not treat those examples as mandatory architecture.

Do not delete existing repository files merely because they are unrelated to the Skill.

## Phase 6 — Validate the Setup

After installation:

1. Confirm that `SKILL.md` exists in the correct Skill directory.
2. Verify that all required local references resolve.
3. Confirm that existing root instructions remain intact.
4. Verify that engineering documentation is discoverable.
5. Check for redundant or conflicting instructions.
6. Validate the Skill against available tooling.
7. Verify that no existing application behavior was modified.
8. Inspect the Git diff for unexpected changes.

Do not install application dependencies or change runtime configuration unless setup genuinely requires it and the change is justified.

## Phase 7 — Existing Repository Assessment

If this is an existing application, perform an initial read-only engineering assessment.

Identify:

- Current technology stack
- Major frontend and backend components
- Existing architectural patterns
- Available tests
- Important business rules
- Known architectural risks
- Missing engineering documentation

Use confirmed findings to initialize the SRS.

Do not redesign, refactor, or rewrite the application as part of this setup.

Where evidence is missing, mark the requirement or implementation status as unverified.

## Phase 8 — Final Report

After completing setup, provide:

1. Final repository folder structure.
2. Files created, moved, or modified.
3. Files intentionally excluded and why.
4. Confirmation of Skill discovery or any harness compatibility limitations.
5. Documentation initialization status.
6. Conflicts or missing requirements requiring attention.
7. How to invoke the Skill during future development.

## Restrictions

- Do not overwrite existing documentation without inspection.
- Do not change application business logic.
- Do not introduce unrelated dependencies.
- Do not deploy the application.
- Do not push directly to protected branches.
- Follow the repository's existing branch and PR workflow.
- Do not merge changes without authorization.
- Prefer minimal, maintainable configuration.
- Preserve all established engineering decisions.

## Expected Outcome

I want a clean, fully integrated, reusable engineering workflow.

Whenever I request a new application, feature, modification, architectural review, or significant bug fix, the AI should be able to use Engineering SRS Guardian to:

**Understand → Architect → Implement → Verify → Document → Preserve Context**

The process must remain application-agnostic, adapt dynamically to the actual business requirements, and avoid unnecessary engineering complexity.

Proceed with the repository setup and validation. Do not begin feature development.

https://drive.google.com/drive/folders/1GxlmPP24Uy0JBeN85CVq_XFO8p_BlNIy?usp=drive_link
