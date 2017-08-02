# RDO Project Easyfix
The RDO Easyfix project is a collection of issues that we consider
"easy to fix".  It is meant as a way to help people begin contributing
to the RDO project.

## I am new to the RDO Project, How can I contribute?
* Check for open [easyfix issues][easyfix-issues]
* Each issue includes the IRC nick of a [mentor](#mentors).
* Read the issue carefully and go through the links attached to issue.
* If you aren't able to understand, join the IRC channel `#rdo` on [Freenode][].
* Contact the mentor regarding the issue, they will help you move forward.

[easyfix-issues]: https://github.com/redhat-openstack/easyfix/issues
[freenode]: https://freenode.net/

## I want to add an easyfix issue
* Go to [issues][] and file the issue.
* Clearly describe the problem to be solved.
* Include the project name as a tag in the issue title (e.g., a DLRN issue would be tagged with `[DLRN]` as in `[DLRN] Proofread documentation`)
* Add steps to reproduce the problem.
* Add links which will help to understand the problem.
* Add your IRC nickname.
* Add information about where someone can contribute changes.
* Always include a link to the project source code.

[issues]: https://github.com/redhat-openstack/easyfix/issues

## I'm still confused, what should I do?
* Join the [RDO mailing list](https://www.redhat.com/mailman/listinfo/rdo-list) and introduce yourself, or
* Join `#rdo` IRC channel on [Freenode][] and say hello.  Someone is generally around and happy to help.
* The [Packager onboarding guide][onboarding] and [RDO Package Maintainer Guide][maintainer] have useful information.

[onboarding]: https://www.rdoproject.org/documentation/onboarding
[maintainer]: https://www.rdoproject.org/documentation/rdo-packaging

## I want to become mentor, What should I do?
* Add your name and IRC nick to the [mentor list](#mentors)
* Follow the steps in [I want to add an easy fix issue](#i-want-to-add-an-easyfix-issue)

## Checklist for sending your first RDO gerrit Review:

* [ ] Run `git checkout -b easyfix/<#easyfix_issue_number>` to create and checkout to a new branch on the issue you are working
* [ ] Add the changed files using `git add <modified files>` command.
* [ ] Then, run `git commit` command, It will open a editor to write a commit message.
* [ ] In the commit message:
   * [ ] First line: What you have fixed?
   * [ ] Second Line: Fixed for issue `RDO easy Fix issue link`
* [ ] Save the file.
* [ ] Run `git review` to send the RDO gerrit review.
* [ ] If something went wrong, you can run `git commit --amend` to change the commit message.
* [ ] We can download specific RDO gerrit review using `git review -d <RDO review number> `

## Mentors
* Alfredo Moralejo (amoralej)
* Alan Pevec (apevec)
* Chandan Kumar (chandankumar)
* David Moreau Simard (dmsimard)
* Haikel Guemar (number80)
* Jakub Ružička (jruzicka)
* Javier Pena (jpena)
* Rich Bowen (rbowen)
* Lars Kellogg-Stedman (larsks)
* Jon Schlueter (jschlueter/yazug)
