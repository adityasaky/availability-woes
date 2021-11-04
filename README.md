# availability-woes

Incidents, high profile or otherwise, where build systems or package installations were impacted due to dependencies being unavailable.

There has been a lot of chatter about `left-pad`'s removal a few years ago, and that's often the cited example for keeping track of dependencies, explicit and transitive. However, it is important to record other similar incidents to improve the integrity of dependency graphs across ecosystems.

## Incidents

These are examples of packages being unavailable that have occurred already.

| Package | Report |
| ------- | ----- |
| left-pad | [Report](incidents/left-pad.md) |
| mimemagic | [Report](incidents/mimemagic.md) |
| Integer Set Library | [Report](incidents/libisl.md) |
| chef-api, chef-sugar, community-zero, stove | [Report](incidents/chef.md) |
| go-bindata | [Report](incidents/go-bindata.md) |

## Things to Watch

These are packages where some yanking is common, or people have faced "localised" issues due to versions being unavailable.

| Package | Report |
| ------- | ----- |
| ring | [Report](watch/ring.md)|

## Yank Policies

| Ecosystem | Report |
| --------- | ------ |
| Python Packaging Index (PyPI) | [Report](repository-policies/pypi.md) |
| NPM | [Report](repository-policies/npm.md) |
| Cargo | [Report](repository-policies/cargo.md) |

### TODO

The following ecosystems should be studied and summarized in this repository. If you'd like to submit a summary or add a new ecosystem not mentioned here, please open a pull request!

| Ecosystem |
| --------- |
| Go Modules |
| RubyGems |
| Maven Central |

## Unavailable, but not Dependencies

These are incidents where there _weren't_ dependencies unavailable causing build failures, but other packages becoming unavailable due to one reason or another. It is still important to document them as similar situations may well occur to packages meant to be used as dependencies.

| Package | Report |
| ------- | ------ |
| youtube-dl | [Report](incidents/youtube-dl.md)

## Contributing

Please open an issue or a pull request if any of the summaries here are incorrect or outdated. Also, please open pull requests if you'd like to submit an incident not listed here, or if there's an ecosystem that should be studied in the context of potential for availability issues.
