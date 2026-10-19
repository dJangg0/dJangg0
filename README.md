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

