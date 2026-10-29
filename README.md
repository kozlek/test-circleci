# test-circleci

A probe of what a CircleCI job can read about the pull request it builds:
the branch, the commit (`CIRCLE_SHA1`: the pull request's head, or a merge
commit?), and the pull request's base, which CircleCI publishes only as a
pipeline value on GitHub App pipelines.

The `probe` job prints those values, the commit checked out and its parents,
and when it started.
