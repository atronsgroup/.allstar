# Allstar configuration for Atrons Group

[Allstar](https://github.com/ossf/allstar) is a security-policy GitHubApp. It is
installed on this org, and this repo contains the configuration for that app. It
is configured to create issues on repos that do not comply with the configured
policy.

## Policy Configuration
These are the expected settings to be in compliance

### [Branch Protection](branch_protection.yaml)

| **Policy**              | **Description**                                             | **Value** |
|-------------------------|-------------------------------------------------------------|-----------|
| enforceDefault          | enforce policy on default branch                            | `true`    |
| requireApproval         | enforce approval on PRs                                     | `true`    |
| requireCodeOwnerReviews | enforce code owner reviews on PRs                           | `true`    |
| approvalCount           | number of required PR approvals                             | `1`       |
| dismissStale            | require PR approvals be dismissed when a PR is updated      | `true`    |
| blockForce              | block force pushes                                          | `true`    |
| requireUpToDateBranch   | require that branches must be up to date before merging     | `true`    |
| enforceOnAdmins         | apply the branch protection rules on administrators as well | `true`    |
| requireSignedCommits    | require signed commits on protected branches                | `true`    |

### [Binary Artifacts](binary_artifacts.yaml)

- Binary artifacts not allowed.

### [Outside Collaborators](outside.yaml)

- Push access not allowed.
- Admin access not allowed.

### [SECURITY.md](security.yaml)

- SECURITY.md required.
