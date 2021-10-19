# npm

npm is the default package management system for Node.js, and has been adopted by the broader JavaScript ecosystem.

## Yanking or Deletion of Versions

Starting from January 2020, npm allows developers to unpublish versions for the first 72 hours after release if they have no public dependents. After 72 hours, they can still be unpublished if they fit certain criteria:
1. The package must have no dependents in the public registry
2. The package must have fewer than 300 downloads over the past week
3. The package must have a single owner / maintainer

After a particular version has been unpublished, it can't be reused again. Instead, a new version number must be used for subsequent releases.

Prior to January 2020, the guidelines had the cut-off time at 24 hours after publishing a version. The policy didn't automatically check for public dependents or the number of downloads. After 24 hours, all requests received manual attention from npm support, who checked if other installs were affected by removing the version in question.

## Deletion of Projects / Potential for Squatting

npm's policies around unpublishing versions extend to the package as a whole. Based on a previous blog post, published in the wake of [left-pad](../incidents/left-pad.md), if a package is entire unpublished, npm publishes a placeholder package as a security measure against squatting. The repository also allows other users to publish a package with the same name after a manual application via email. It is unclear how these users are vetted, since the blog post also says that they generally grant these requests.

npm has a separate dispute resolution process for transferring names in situations where names of a package are confusing or misleading, or is squatting to occupy the namespace. Transferring names of packages, organizations, and users all require opening of a support ticket, which indicates that the process involves a human in the loop. The policy is a little unclear on the metrics used to identify who the rightful owner of a disputed name is (outside of situations with trademarks). For example, package names are considered squatted if the package has "no genuine function", which is not very specific.

## Sources

1. npm Unpublish policy: https://docs.npmjs.com/policies/unpublish, archived at https://archive.md/vljlI
2. Changes to unpublish policy (after left-pad): https://blog.npmjs.org/post/141905368000/changes-to-npms-unpublish-policy, archived at https://archive.md/PsBDf
3. Changes to unpublish policy in January 2020: https://blog.npmjs.org/post/190553543620/changes-to-npmunpublish-policy-january-2020, archived at https://archive.md/HRft2
4. npm's security placeholder package: https://github.com/npm/security-holder, archived at https://archive.md/0VSKS
5. npm's Dispute Resolution policy: https://docs.npmjs.com/policies/disputes, archived at https://archive.md/VpQC3