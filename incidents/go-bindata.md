# go-bindata

In 2018, GitHub user "jteeuwen" deleted their account. The account maintained a popular Go package called go-bindata. This incident predated Go Modules, and therefore builds began failing as the dependency was fetched directly from the GitHub repository.

In response, someone unaffiliated with "jteeuwen" pushed a copy of the dependency they had, so that their (and others') builds would stop failing. This also highlighted a potential flaw with GitHub's policies around the usernames of deleted accounts being up for grabs for registration, as well as Go's policies at the time with relying on version control systems for distributing dependencies.

Some time after, GitHub announced their plan to retire the namespaces of popular repositories, specifically those that had 100 clones in the week leading up to the account deletion. While the account name can still be registered, those new accounts can't create repositories with the same name.

## Sources

1. Statement by new owners of the "jteeuwen" account: https://github.com/jteeuwen/go-bindata/issues/5, archived at https://archive.md/VRPBO
2. Reddit discussion of the incident: https://www.reddit.com/r/golang/comments/7vv9zz/popular_lib_gobindata_removed_from_github_or_why/, archived at https://archive.md/vVL76
3. The Register article: https://www.theregister.com/2018/02/10/github_account_name_reuse/
4. GitHub policy regarding retiring popular namespaces: https://github.blog/2018-04-18-new-tools-for-open-source-maintainers/#popular-repository-namespace-retirement, archived at https://archive.md/O0poW