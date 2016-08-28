# Contributing

## Issues and Bugs

Github will be the source of bug/issue tracking.  All bugs should
include the following in the description

1. Full stack trace if applicable
2. A minimal example of reproducing the bug.  Please make this the absolute smallest amount of code to reproduce it.
3. OS, language version, package version, and any other relevant environment configurations
4. (optional) Reproduce the bug using a Docker container and post the code as a Github Gist.

## Commits and Commit Messages

Whenever possible, a commit should contain a single
feature or bug fix.  The bug fix/feature should not be
spread across multiple commits.  If there are checkpoint commits
they should be squashed to a single commit before pushing
to the remote.

Commit messages should be detailed and explain exactly what is
going on.  [This article](http://chris.beams.io/posts/git-commit/) details
what is expected for commit messages.  The summary is below:

1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how

## Pull Requests

1. Keep your pull requests to a single issue/feature
2. Include/update unittests for all impacted areas.  Bug fixes should include a test that would break before the bug.
3. Follow the criteria on writing commits above
