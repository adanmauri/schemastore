[![ColPrac: Contributor's Guide on Collaborative Practices for Community Packages](https://img.shields.io/badge/ColPrac-Contributor's%20Guide-blueviolet)](https://github.com/SciML/ColPrac)

We follow the ColPrac guide for collaborative practices. New contributor should make sure to read that guide.
Following here are some additional clarifications and practices we follow.

Thanks for taking the plunge!

## Reporting Issues

* It's always good to start with a quick search for an existing issue to post on,
  or related issues for context, before opening a new issue
* Including minimal examples is greatly appreciated

## Contributing

* If you are a new contributor and would like to get a guidance on what area
  you could focus your first PR please do not hesitate to ask and the developers
  will help you with picking a topic matching your experience.
* Feel free to open, or comment on, an issue and solicit feedback early on,
  especially if you're unsure about aligning with design goals and direction,
  or if relevant historical comments are ambiguous.
* Aim for atomic commits, if possible, e.g. `change 'foo' behavior like so` &
  `'bar' handles such and such corner case`,
  rather than `update 'foo' and 'bar'` & `fix typo` & `fix 'bar' better`.
* It is recommended to disable GitHub Actions on your fork; check Settings > Actions.
* A PR with breaking changes should have `[BREAKING]` as a first part of its name.
* If you make a PR please try to avoid pushing many small commits to GitHub in
  a sequence as each such commit triggers a separate CI job, which takes over
  an hour. This has a consequence of making other PRs in packages from the JuliaData
  ecosystem wait for such CI jobs to finish as they share a common pool of CI resources.

## Git Recommendations For Pull Requests

* Avoid working from the `main` branch of your fork, creating a new branch will make it
  easier if DataFrames.jl `main` branch changes and you need to update your pull request;
* All PRs and issues should be opened against the `main` branch not against the current release;
* If any conflicts arise due to changes in DataFrames.jl `main` branch, prefer updating your pull
  request branch with `git rebase` (rather than `git merge`), since the latter will introduce a merge 
  commit that might confuse GitHub when displaying the diff of your PR, which makes your changes more 
  difficult to review. Alternatively use conflict resolution tool available at GitHub;
* Please try to use descriptive commit messages to simplify the review process;
* Using `git add -p` or `git add -i` can be useful to avoid accidentally committing unrelated changes;
* Maintainers get notified of all changes made on GitHub. However, what is useful is writing a short
  message after a sequence of changes is made summarizing what has changed and that the PR is ready
  for a review;
* When linking to specific lines of code in discussion of an issue or pull request, hit the `y` key
  while viewing code on GitHub to reload the page with a URL that includes the specific commit that 
  you're viewing. That way any lines of code that you refer to will still be correct in the future, even 
  if additional commits are pushed to the branch you are reviewing;
* Please make sure you follow the code formatting guidelines when submitting a PR;
  Also preferably do not modify parts of code that you are not editing as this makes
  reviewing the PR harder (it is better to open a separate maintenance PR
  if e.g. code layout can be improved);
* If a PR is not finished yet and should not be reviewed yet then it should be opened as DRAFT 
  (in this way maintainers will know that they can ignore such PR until it is made non-draft or the author
  asks for a review).
