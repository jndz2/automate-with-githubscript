# automate-with-githubscript

* [Automate GitHub using GitHub-Script](https://learn.microsoft.com/en-us/training/modules/automate-github-using-github-script/?source=learn)

* [GitHub-Script Repo](https://github.com/actions/github-script)


## How is using GitHub Script different from octokit/rest.js?
The main difference in usage is that GitHub Script provides you with a pre-authenticated octokit/rest.js client named github.

So instead of:
```js
octokit.issues.createComment({
```
You would use:

```js
github.issues.createComment({
```

In addition to the github variable, the following variables are also provided:

* context is an object containing the context of the workflow run
* core is a reference to the @actions/core package
* io is a reference to the @actions/io package
