# Definition of Done — For a Story

## A story is done when...

<details>
<summary><b>🚦 1. Code has been <i>peer-reviewed</i> and <i>merged</i> to a hosted code repository</b></summary>

_Writing Code_

- ⭐ It should go without saying: The source code for the project is stored in a hosted, version-controlled, code repository
- ⭐ New code enters the codebase via a Pull Request (PR), also known as a Merge Request (MR)
- ⭐⭐ New code improves the codebase, so that it is in a better state than it was before

_Pull Request Checklist_

- ⭐ There is a Pull Request checklist (possibly several, one for each type of change)
- ⭐ The PR checklist includes the elements of a well-formed PR (meaningful commit messages, no accidental changes, tests passing, etc)
- ⭐⭐ The PR checklist incorporates many items from this Definition of Done (especially those related to PR creation, quality gates, testing, and documentation)
- 👎 Don't make the PR checklist _too_ complicated, otherwise developers may get lazy and stop filling it out
- 👎 Don't let the PR checklist get out of date

_Creating the Pull Request_

- ⭐ The Pull Request checklist is filled out by the author of the PR
- ⭐⭐ The PR is concise enough for a reviewer to be able to understand the code with relative ease
- ⭐⭐ The PR is a fully-functioning unit of change, and is production ready (able to be deployed to production without issues, possibly in an inactive state)
- ⭐⭐⭐ Each commit in the PR is for a single purpose and has a clear commit message (sometimes called "hiding the sausage making", a somewhat controversial topic)

_Reviewing the Pull Request_

- ⭐ The Pull Request is reviewed by 2 other engineers
- ⭐ One of the reviewers is a core maintainer of the project
- ⭐ The PR checklist is reviewed for accuracy
- ⭐⭐ The code is reviewed line by line, and understood by the reviewer
- ⭐⭐ At the discretion of the reviewer, the code and/or tests are executed ("kicking the tires")
- ⭐⭐⭐ For a more rigorous and opinionated treatment on the topic of developer collaboration, see [The Main Gig](https://github.com/eugenious/the-main-gig)
- 👎 Code reviewers just "rubber-stamp" the change without actually reviewing it
- 👎 Too many "back and forth" comments on a PR usually indicates that the PR has not been adequately prepared

</details>

<details>
<summary><b>🔬 2. Code has passed <i>quality gates</i></b></summary>

- ⭐ Code is checked for issues (formatting, linting, potential bugs) using an automated tool
- ⭐ No new security findings (including open source vulnerabilities)
- ⭐ All tests are passing
- ⭐ New code has adequate unit test code coverage (meets minimum requirements)
- ⭐⭐ Quality gates are all executed automatically and block a PR from being merged if any are failing
- ⭐⭐⭐ Unit test code coverage of 100% (yes, that's the goal!)

</details>

<details>
<summary><b>🏄 3. Code has been <i>deployed</i> to a testing environment</b></summary>

- ⭐ Deployable artifacts are created using a Continuous Integration server (not on a local workstation!)
- ⭐ Deployable artifacts are stored in an artifact repository
- ⭐ Code is deployed from an artifact repository to a hosted test environment (non-production)
- ⭐⭐ Code is automatically deployed once it has been merged into the codebase
- ⭐⭐⭐ Quality gates are all executed automatically and block a deployment if any are failing

</details>

<details>
<summary><b>🧪 4. There are <i>tests</i> that prove all scenarios and acceptance criteria are satisfied</b></summary>

- ⭐ Acceptance criteria (applies to all stories in the project) are written out and understood by the team, and may include items such as localization, logging, analytics, etc...
- ⭐ All test scenarios for the story are written out in detail (ideally, using Given-When-Then syntax
- ⭐ Features are considered done only when there are passing tests
- ⭐ Test scenarios are gathered into a suite for future use
- ⭐⭐ The tests results are kept somewhere for future reference
- ⭐⭐ Automated tests are executed against the test environment (not just locally)
- ⭐⭐⭐ **All** integration tests are automated
- ⭐⭐⭐ Integration tests are executed automatically by a Continuous Integration system

</details>

<details>
<summary><b>📝 5. There is <i>documentation</i></b></summary>

- ⭐ The documentation is appropriate for the project
- ⭐ The documentation is accurate and up-to-date
- ⭐ The documentation is easy to find
- ⭐ The documentation is in a suitable format
- 👎 There is such a thing as too much of a good thing, so don't over-document

</details>

<details>
<summary><b>🏁 6. Work has been reviewed and <i>accepted</i> by the product owner</b></summary>

- ⭐ The product owner has tried the feature or has been given a demo
- ⭐⭐ The product owner has reviewed the test scenarios and test results
- ⭐⭐ The product owner confirms that all details of the story are accurate (description is complete, all subtasks are closed, fix version is assigned, etc...)
- ⭐ Finally, the product owner marks the story as done!

</details>
