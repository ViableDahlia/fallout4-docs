Using Git commit good practices is one of the most effective ways to maintain a healthy, scalable, and collaborative codebase.

Here is a breakdown of **why** good commits matter and **what** you should include in them.

---

### Why Good Commits Matter

1. **Easier Code Reviews:** Smaller, well-documented commits allow reviewers to understand your thought process block-by-block rather than wading through a massive "code dump."
2. **Simplified Troubleshooting (`git blame` & `git log`):** When a bug is discovered months later, a clear commit message acts as a historical document explaining *why* a specific line of code was written or changed.
3. **Efficient Bug Hunting (`git bisect`):** If you need to use `git bisect` to find the exact commit that introduced a bug, having isolated, working commits ensures you can pinpoint the error quickly.
4. **Automated Changelogs:** Many teams use tools that automatically generate release notes and changelogs directly from well-formatted commit messages.

---

### What to Add to Commits (The "Atomic" Rule)

A good commit consists of two parts: **The Right Code** and **The Right Message**.

#### 1. The Code: Keep it "Atomic"

An atomic commit means **one commit equals one logical change**.

* **Do:** Group a new feature and its corresponding tests in one commit.
* **Don't:** Mix a feature implementation, a typo fix in an unrelated file, and a dependency update into a single commit.
* *Tip:* If you’ve done too much work at once, use `git add -p` to interactively stage only specific parts of your files.

#### 2. The Message: Structure It Correctly

A professional commit message follows a standard structure: a short summary, an optional detailed body, and optional metadata/footers.

* **The Subject Line (The "What"):**
* Limit it to **50 characters** or less.
* Capitalize the first letter.
* Do not end with a period.
* Use the **imperative mood** (e.g., "Add user authentication" instead of "Added user authentication" or "Adds user authentication"). *Rule of thumb: It should complete the sentence: "If applied, this commit will... [your message]."*


* **The Body (The "Why" and "How"):**
* Separate the subject line from the body with a blank line.
* Focus on **why** the change was necessary and **how** it addresses the issue, rather than just repeating *what* the code does (the code itself shows the "what").
* Wrap lines at around 72 characters.


* **The Footer (The Metadata):**
* Use this to reference issue trackers or pull requests (e.g., `Fixes #142` or `Closes PROJ-12`).



---

### A Widely Used Standard: Conventional Commits

Many development teams follow the **Conventional Commits** specification. It adds a lightweight structure to your subject lines by prefixing them with a **type**:

* `feat:` A new feature for the user.
* `fix:` A bug fix for the user.
* `docs:` Changes to the documentation.
* `style:` Formatting, missing semi-colons, etc. (no production code change).
* `refactor:` Refactoring production code (e.g., renaming a variable, optimizing a function).
* `test:` Adding missing tests or correcting existing tests.
* `chore:` Updating build tasks, package manager configs, etc.

#### Example of a Great Commit Message:

```text
feat: add password strength validation to signup

Implement a zxcvbn-based validation check during user registration 
to ensure users choose stronger passwords. This reduces the risk 
of credential stuffing attacks.

Closes #482

```