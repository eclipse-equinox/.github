# Contributing to Eclipse Equinox

Thanks for your interest in this project.

In all your interactions please keep in mind that Eclipse is a fully open and community driven project where everybody can participate. Many contributors are volunteers that contribute in their free time or address the issues that are relevant for them. Just because this issue has not yet been addressed doesn't mean we don't appreciate your report.

Possible ways how to resolve this issue are:
- Provide a pull-request to fix this issue by yourself.
Quality contributions are always very welcome! See the contribution guidelines in this repositories or organization. If you have further question don't hesitate to ask.
- Convince us project committers (or somebody else) that this is a urgent issue that affects all users in general.
But because this issue is inactive for some time the chances that this is urgent is usually not very high.
- Wait until all of a sudden somebody else finds this issue interesting and solves it.
But it is possible that you have to wait for quite some time, if not forever.
- Hire a professional to solve this issue for you.
There are freelancers who offer commercial services to enhance Eclipse for you. If you are interested please ask and we can get you in touch.

### Setting up GitHub account

Create an account at github.com using the same email id used for [Eclipse Community account](https://accounts.eclipse.org/user). If you don't have an Eclipse Community account, please create one.

In you already have an account, add the email you've used to register to Eclipse Community to your GitHub account using <https://github.com/settings/emails>.
Add GitHub account id to contributor's [Eclipse Community account](https://accounts.eclipse.org/user) under social media links section.

If contributor is already a commiter in any of the projects, a mail containing invite to join 
that project's github organisation will be received within 2 hours. The contributor should accept the invite to maintain committer status in the github organisation

To create commits it is recommended to add ssh public keys to github account. This can be done using <https://github.com/settings/keys>.


### Create an Eclipse Development Environment

[![Create Eclipse Development Environment for Equinox](https://download.eclipse.org/oomph/www/setups/svg/Equinox.svg)](
https://www.eclipse.org/setups/installer/?url=https://raw.githubusercontent.com/eclipse-equinox/equinox/master/releng/org.eclipse.equinox.releng/EquinoxConfiguration.setup&show=true
"Click to open Eclipse-Installer Auto Launch or drag into your running installer")

[![Create Eclipse Development Environment for Equinox P2](https://download.eclipse.org/oomph/www/setups/svg/P2.svg)](
https://www.eclipse.org/setups/installer/?url=https://raw.githubusercontent.com/eclipse-equinox/p2/master/releng/org.eclipse.equinox.p2.setup/EquinoxP2Configuration.setup&show=true
"Click to open Eclipse-Installer Auto Launch or drag into your running installer")

### Recommended workflow

Recommended way of developing code is inside a fork of the man repository (see [Fork and pull model](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/getting-started/about-collaborative-development-models#fork-and-pull-model) in the github documentation).

Here are the steps:

1. Use the fork button available on the github repository page to create a forked repository under your github account.
2. If fork already exists, click of fetch upstream to get latest source code.
3. Clone the forked repository to eclipse workspace. Repository link can be found by clicking code button on the top right in "<> code" tab
4. Create a local branch
5. Delevelop fix
6. Commit code changes to local branch. Make multiple commits if necessary as history can be retained.
7. Once the fix is ready, push the branch to origin(in this case forked repositoy)
8. Open forked repository page, switch to the branch where the fix is developed, a new option appears just below code button "Contribute" Click on this to open "Pull Request" also called PR.
9. Verify the branch information like contributing to master or contributiong to any other branch and list of commits. If every thing OK, please click on "Create pull request" button at the bottom right
10. Can add reviewers if necessary.
11. Any commits pushed to the devlopment branch(used to create PR) automatically gets added to opened PR.
12. Reviewer can review PR on the github portal itself or fetch the PR using egit menu "Fetch github PR"
13. All PRs will get verified for eca and PR validations(same as gerrit validation)
14. Once the PR is approved there two options to merge. Can select either of these based on the requirement the following are recommendations only. Need to select based on the requirement

  * Rebase and Merge (retains commit history from PR useful in developing a feature)
  * Squash and Merge (All commits in PR gets squashed in to a single commit useful in bug fixes)

15. Once PR gets merged the development branch used for the PR can be deleted.

Commit message recommendations

  \<issue title\> \#\<issue number\>
  
  Example: The eclipse-test-framework deliverable contains unsigned bundles \#32
  
  Again this is a recommendation on the issue title part. Instead of issue title, if needed provide a concise description of changes.
  Please do not forget to add issue number to the commit message. This is used to link with github issue.

## Eclipse Contributor Agreement

Before your contribution can be accepted by the project team contributors must
electronically sign the Eclipse Contributor Agreement (ECA).

* <https://www.eclipse.org/legal/ECA.php>

Commits that are provided by non-committers must have a Signed-off-by field in
the footer indicating that the author is aware of the terms by which the
contribution has been provided to the project. The non-committer must
additionally have an Eclipse Foundation account and must have a signed Eclipse
Contributor Agreement (ECA) on file.

For more information, please see the Eclipse Committer Handbook:
<https://www.eclipse.org/projects/handbook/#resources-commit>.

## Contact

Contact the project developers via the project's "dev" list.

* <https://dev.eclipse.org/mailman/listinfo/equinox-dev>
