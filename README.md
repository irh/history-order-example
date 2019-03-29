This repo demonstrates an issue with the ordering of commits in Github's Pull Requests.

[This PR](https://github.com/irh/history-order-example/pull/1) shows a series of commits which are displayed in the correct order.

[This PR](https://github.com/irh/history-order-example/pull/3) shows the same commits, which are displayed in the incorrect order, due to the commits being sorted by 'commit date'.

The commits in both branches are in the same topological order, so its suprising to find them presented differently in the PRs.

When rebasing a branch, it can make sense to reorder the commits so that the branch has a clearer narrative, which helps the reader of the branch to understand its contents.

Sorting by anything other than topological order breaks this flow, which can cause a branch reviewer to misunderstand the author's intentions.
