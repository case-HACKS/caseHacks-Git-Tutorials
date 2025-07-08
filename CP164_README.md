# 🚀 GitHub Basics for CP164: Clone, Fork & Pull
#### Brought to you by [case]hacks 💻💡

> Congrats on wrapping up **CP164: Data Structures**! 🎉  
> You’ve just leveled up your problem-solving and coding skills, now let’s add some more Git commands to your toolkit. This guide is part two of our GitHub basics series. If you’ve already completed the [CP104 GitHub Basics](https://github.com/your-org/cp104-github-basics) on `push`, `add`, and `commit`, you’re in the right place.  
>  
> In this CP164 edition, you’ll learn how to:
> - 🌀 **Fork** a repo (make your own copy on GitHub)  
> - 💻 **Clone** it to your computer  
> - 🔁 **Pull** changes from the original repo  

Let’s go!

---

## What You’ll Need
- A GitHub account
- Git installed on your machine
- [GitHub Desktop](https://desktop.github.com/) (optional, but helpful)
- Completed CP104 GitHub basics or basic knowledge of Git

---

## Step 1: Fork this repository  

<details>
<summary>🤔 What does <code>fork</code> mean?</summary>

Forking means making a **copy of someone else's repository** to your own GitHub account.

This is useful when:
- You want to contribute to a project without affecting the original.
- You need your own workspace to make changes.
- You want to sync updates from the original repo later (see: `pull`).

</details>

1. Click the **Fork** button in the top-right corner.
2. Now you’ll see your own version: `your-username/cp164-github-basics`.


## Step 2: Clone your fork  

<details>
<summary>🤔 What does <code>clone</code> mean?</summary>

Cloning means **downloading a GitHub repository to your own computer** so you can edit files locally.

You’ll use this command so you can make changes using your code editor.

</details>

```bash
git clone https://github.com/your-username/cp164-github-basics.git
cd cp164-github-basics
```

## Step 3: Check your remote

<details>
<summary>🤔 What is a <code>remote</code>?</summary>

A remote is a version of your project that's hosted somewhere else — like GitHub.

- `origin`: your personal copy (fork)
- `upstream`: the original repo you forked from

You can use Git commands to sync between them.

</details>

```bash
git remote -v
```

You should see something like:

```
origin  https://github.com/your-username/cp164-github-basics.git (fetch)
origin  https://github.com/your-username/cp164-github-basics.git (push)
```


## Step 4: Connect to the original repo  

<details>
<summary>🤔 What does <code>upstream</code> mean?</summary>

`upstream` refers to the **original repo you forked from**. You use this to pull in updates that have been made to the original project.

This helps you stay in sync!

</details>

```bash
git remote add upstream https://github.com/casehacks/cp164-github-basics.git
```

Then confirm:

```bash
git remote -v
```


## Step 5: Pull changes from upstream  

<details>
<summary>🤔 What does <code>pull</code> mean?</summary>

Pulling means **downloading and merging changes** from a remote repository into your current branch.

You usually pull from:
- `origin` (your fork)
- or `upstream` (the original)

</details>

```bash
git fetch upstream
git merge upstream/main
```


## Step 6: Make changes & commit  

<details>
<summary>🤔 What does <code>commit</code> mean?</summary>

A commit is a saved snapshot of your changes. Think of it like hitting "Save + Version History" at the same time.

</details>

```bash
echo "hello from cp164!" >> sample.txt
git add .
git commit -m "Added my greeting"
```

## Step 7: Push your changes  

<details>
<summary>🤔 What does <code>push</code> mean?</summary>

Pushing sends your commits (saved changes) from your computer back to your fork on GitHub.

</details>

```bash
git push origin main
```

## You did it!
You’ve now completed both **parts of GitHub basics** with [case]hacks:
- ✅ CP104: Push, Add, Commit  
- ✅ CP164: Clone, Fork, Pull  

You're well on your way to collaborating like a pro.

---
## Additional Resources

Here are some additional resources too help you out!
- (Link our video once it's made)
- [Git Cheatsheet by GitHub](https://education.github.com/git-cheat-sheet-education.pdf) 

## Acknowledgements

This quick guide was brought to you by **[case]hacks**!

Make sure to keep an eye on our repositories! We will be posting guides and videos on how to use the code you learned in class and turn it into actual projects!
[case]Hacks (our website link)

Happy Coding 💛!
