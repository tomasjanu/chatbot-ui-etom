# Updating a Forked Repository from the Original Repository

When you fork the repository [chatbot-ui](https://github.com/mckaywrigley/chatbot-ui), you create a separate copy of the original repository. If the original repository is updated and you want to include these changes in your fork, follow these steps:

## 1. Add the Original Repository as a Remote

First, list the current configured remote repository for your fork:

```
git remote -v
```

Then, add the [chatbot-ui](https://github.com/mckaywrigley/chatbot-ui) repository as a remote (typically called `upstream`):

```
git remote add upstream https://github.com/mckaywrigley/chatbot-ui.git
```

## 2. Fetch the Changes from the Original Repository

Fetch the branches and their respective commits from the upstream repository:

```
git fetch upstream
```

## 3. Merge the Changes

Check out your fork's local default branch (usually `master` or `main`):

```
git checkout master
```
Or for `main`:
```
git checkout main
```

Merge the changes from the [chatbot-ui](https://github.com/mckaywrigley/chatbot-ui)'s default branch into your local default branch:

```
git merge upstream/master
```
Or for `main`:
```
git merge upstream/main
```

## 4. Push the Updates to Your Fork on GitHub

After merging the changes locally, push them to update your fork on GitHub:

```
git push origin master
```
Or for `main`:
```
git push origin main
```

Now your fork should be up-to-date with [chatbot-ui](https://github.com/mckaywrigley/chatbot-ui).

