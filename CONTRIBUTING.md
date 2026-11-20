# Contributing

## Code of conduct

All participants of the CAMARA Project must abide by the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) derived from [Contributor Covenant](https://www.contributor-covenant.org/). Only by respecting each other can we develop a productive, collaborative community. Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting _project email address_ and/or a Project maintainer.

We appreciate your courtesy of avoiding political questions here. Issues which are not related to the project itself will be closed by our Project maintainers.

## Engaging in our project

The process how contributions are progressed in CAMARA is defined in [ProjectStructureAndRoles.md](https://github.com/camaraproject/Governance/blob/main/ProjectStructureAndRoles.md#project-structure). In the present document you can find some detailed information.

If you need a general basic and friendly introduction to git and GitHub, you are encouraged to watch the ["GitHub for poets"](https://www.youtube.com/watch?v=BCQHnlnPusY) series.

The starting point of any contribution should be an issue or a pull request:

* If you have a trivial fix or improvement, go ahead and create a pull request, addressing (with `@...`) a suitable maintainer of the respective repository (see the specific CODEOWNERS.MD or MAINTAINERS.MD file of the Sub Project you want to contribute to) in the description of the pull request.

*	If you have a bigger change (esp. that requires new documents) then please open an issue in the respective repository (and upload all initial documents in it).

*	If you are unsure, please reach out to the Sub Project community. This will avoid unnecessary work and surely give you and us a good deal of inspiration.

## Working on issues

Should you wish to work on an issue, please claim it first by commenting on the GitHub issue that you want to work on. This is to prevent duplicated efforts from other contributors on the same issue.

If you have questions about one of the issues, please comment on them, and one of the maintainers will clarify.

Please provide as much context as possible when you open an issue. The information you provide must be comprehensive enough to reproduce that issue for the assignee. Therefore, contributors may use but aren't restricted to the issue template provided by the project maintainers.

### Guidance for closing issues
* As per the [ProjectCharter](https://github.com/camaraproject/Governance/blob/5fc802713d71a51da64136f692b16ed620eeffa5/ProjectCharter.md), The default decision making mechanism for the CAMARA Project is [lazy consensus](https://couchdb.apache.org/bylaws.html#lazy). This means that any decision on technical issues is considered supported by the team as long as nobody objects based on substantiated technical grounds.
* Once consensus is achieved, an issue may be closed by the original author or by a maintainer in the sub-project (if not closed by a Pull Request merge, where the issue is linked as getting fixed, see below)
* Closing an issue should include a comment on how it was resolved or why it won't be resolved


* A sub-project participant may object to closure of an issue if they believe consensus was not reached, in which case they may reopen the issue, stating they believe consensus has not been reached.
* Closure of an issue may require closure of a Pull Request which only fixed that single (now closed) issue.


## Contributing Code

You are welcome to contribute code in order to fix a bug or to implement a new feature.

The following rule governs code contributions:

* Contributions must be licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0)
* Newly created files must start with an instantiated version to the [file-header.txt](https://github.com/camaraproject/Governance/blob/main/declarations/templates/file-header.txt).
* At least if you add a new file to the repository and you're not a Project participant, send an onboarding email to <all+subscribe@lists.camaraproject.org>.

## Contributing Documentation

You are welcome to contribute documentation to the project.

The following rule governs documentation contributions:

* Contributions must be licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
* Only exception are contributions to the Marketing Working Group in the folder [https://github.com/camaraproject/Marketing](https://github.com/camaraproject/Marketing). For that the [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/legalcode.txt) shall apply.

* At least if you add a new documentation to the repository and you're not a Project participant, add your name into the [PARTICIPANTS](./PARTICIPANTS.MD) file or send an onboarding email to <all+subscribe@lists.camaraproject.org>.

## Creating Branches

Branches allow to develop features, fix bugs, or safely experiment with new ideas in a contained area of our repository. If you need a friendly video introduction to git branching, please try [part two of "GitHub for Poets"](https://www.youtube.com/watch?v=oPpnCh7InLY) on Youtube, you may also read GitHub's ["Creating and deleting branches within your repository"](https://docs.github.com/en/articles/creating-and-deleting-branches-within-your-repository) for a deep dive. 

Creating branches within the project repositories itself requires write access to the repository and will done by code owners for specific purposes. For contribution into the branches of the project the "fork and pull model" is used. You need to create the branch for your contribution within a fork of the repository (see [part three of "GitHub for Poets"](https://youtu.be/_NrSWLQsDL4) for an friendly explanation or ["Working with forks"](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks).

## Creating Pull Requests

For adding modifications to a branch in CAMARA, a pull request has to be initiated. When you open a pull request, you're proposing your changes and requesting that someone reviews and pulls in your contribution and merges them into their branch. Pull requests show diffs, or differences, of the content from both branches. The changes, additions, and subtractions are shown in different colors.

Anyone with read access to a repository can create a pull request. You can specify which branch you'd like to merge your changes into when you create your pull request. You can link a pull request to an issue to show that a fix is in progress and to automatically close the issue when someone merges the pull request (see ["Linking a pull request to an issue"](https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue)).

By using GitHub's @mention feature in your pull request message, you can ask for feedback from specific people.

For more information on pull requests watch the third episode of ["GitHub for Poets"](https://www.youtube.com/watch?v=_NrSWLQsDL4). For a deep dive, see GitHub's docs:
*	[About pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
*	[Propose changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests)
*	[Collaborate with pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)

We kindly ask you to follow the [Pull Request Checklist](#Pull-Request-Checklist) to ensure reviews can happen accordingly.

## Pull Request Checklist

* Work on a fork of the repository.

* Branch from the main branch and, if needed, rebase to the current main branch before submitting your pull request. If it doesn't merge cleanly with main you may be asked to rebase your changes. See also [Keeping your pull request in sync with the base branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/keeping-your-pull-request-in-sync-with-the-base-branch) and [More ways to keep your pull request branch up-to-date](https://github.blog/changelog/2022-02-03-more-ways-to-keep-your-pull-request-branch-up-to-date).

* Commits should be as small as possible while ensuring that each commit is correct independently (i.e., each commit should compile and pass tests).

* Test your changes as thoroughly as possible before you commit them. Preferably, automate your test by unit/integration tests. If tested manually, provide information about the test scope in the PR description (e.g. “Test passed: Upgrade version from 0.42 to 0.42.23.”).

* If your patch is not getting reviewed or you need a specific person to review it, you can @-reply a reviewer asking for a review in the pull request or a comment, or you can ask for a review by contacting the Sub Project community.

* Post review:
  * If a review requires you to change your commit(s), please test the changes again.
  * Amend the affected commit(s) and force push onto your branch.
  * Set respective comments in your GitHub review to resolved.
  * Create a general PR comment to notify the reviewers that your amendments are ready for another round of review.
