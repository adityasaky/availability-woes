# availability-woes

Incidents, high profile or otherwise, where build systems or package installations were impacted due to dependencies being unavailable.

There has been a lot of chatter about `left-pad`'s removal a few years ago, and that's often the cited example for keeping track of dependencies, explicit and transitive. However, it is important to record other similar incidents to improve the integrity of dependency graphs across ecosystems.

If the details of an incident or policy are incorrect or outdated, please open an issue or a pull request!

## Incidents

These are examples of packages being unavailable that have occurred already.

| Package | Report |
| ------- | ----- |
| left-pad | [Report](incidents/left-pad.md) |
| mimemagic | [Report](incidents/mimemagic.md) |
| Integer Set Library | [Report](incidents/libisl.md) |

## Things to Watch

These are packages where some yanking is common, or people have faced "localised" issues due to versions being unavailable.

| Package | Report |
| ------- | ----- |
| ring | [Report](watch/ring.md)|

## Yank Policies

TODO: these are studies of how popular package repositories handle package yanking.

| Ecosystem | Report |
| --------- | ------ |
| Python Packaging Index (PyPI) | [Report](repository-policies/pypi.md) |
| NPM | [Report](repository-policies/npm.md) |
| Cargo | [Report](repository-policies/cargo.md) |
| Go Modules | [Report](#) |

## Unavailable, but not Dependencies

These are incidents where there _weren't_ dependencies unavailable causing build failures, but other packages becoming unavailable due to one reason or another. It is still important to document them as similar situations may well occur to packages meant to be used as dependencies.

| Package | Report |
| ------- | ------ |
| youtube-dl | [Report](incidents/youtube-dl.md)
