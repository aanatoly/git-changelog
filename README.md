# git-changelog
Creates nice change log from closed Github or Bitbucket issues.

I see it as a helper tool for [git flow](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/) development model, since it requires that people

 * open issues
 * reference them in commit messages with `#NN`
 * close issues in time, see [note1](#note1)

See [CHANGELOG.md](https://github.com/aanatoly/git-changelog/blob/master/CHANGELOG.md) of git-changelog itself

------------
## Version: 0.5
Date: 2015-11-30 16:11:26

 * [#13] remove trailng whitespace from issue title
 * [#12] remove trailng whitespace
 * [#8] hide typed password

[#13]: https://github.com/aanatoly/git-changelog/issues/13
[#12]: https://github.com/aanatoly/git-changelog/issues/12
[#8]: https://github.com/aanatoly/git-changelog/issues/8

## Version: 0.4
Date: 2015-11-30 06:33:20

 * [#11] use git-flow release name, if available
 * [#7] fix access to read-only github repos
 * [#6] print non-log data to stderr

[#11]: https://github.com/aanatoly/git-changelog/issues/11
[#7]: https://github.com/aanatoly/git-changelog/issues/7
[#6]: https://github.com/aanatoly/git-changelog/issues/6
------------

-------

##### note1
Github delays closing of the issue, until commit with `closes #NN` merges into
`muster`. Which in our case happends quite rare. So to make issue tracker
reflect real situation, we close it manually.
