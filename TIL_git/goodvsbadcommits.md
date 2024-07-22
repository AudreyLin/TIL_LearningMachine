# Good vs Bad Commits

There are best practices for making commits to ensure that version control stays clean, organized & maintained. A commit is a snapshot of your code at a specific point in time & should remain atomic, focused, and clearly descriptive for context to ensure a good commit. This file summarizes an article (referenced at the bottom).  It's not short or my own findings, but I wanted to have it here for later use.

## Characteristics of a good commit
* Atomic
* Focused
* represents a single logical change
* descriptive commit message: 
    * what the commit does
    * why the change was made
    * enough context without needing to read the code
* Follows conventional commit guidelines
    * uses standard commit guidelines
    * keeps history clean & consistent
    * common prefixes: 
        * feat
        * fix
        * chore
        * refactor
        * docs
* Tested & verified changes to prevent breaking build or workflow for others
* Properly scoped: commits should include all changes related to a specific feature or bug fix, avoiding partial changes that leave codebase in an inconsistent state.

## Characteristics of a bad commit
* Large & unfocused: commits with too many changes are hard to understand & review
* vague or misleading messages: makes tracking changes difficult
* unrelated changes in a single commit - this complicates review process & introduces bugs
* Lack of context - doesn't clarify the reason for changes

## Best Practices for good commits 
* Commit often - not too often
* clear descriptive messages:
    * keep first line under 50 characters
    * keep body under 72 characters
    * eliminate filler words
    * use imparative mood to write
    * specify commit type
    * answer key questions
* use branches effectively
    * new branches for:
        * new features
        * bug fixes
        * experiments
    * pull requests for those branches to facilitate review & merging
* Review & squash commits before merging a branch
    * keep small or fixup commits into logical units to keep the history clean
* Automate testing
    * use continuous integration tools to auto-test code w/ each commit
    * use husky to enforce rules & prevent breaking the configuration

## Conventional commit formats
Maintain consistency with a structured format:
* Type - (kind of change)
* Scope - helps specify area affected by changes
* description - summarize changes
* body - provides details of change
* footer - references or breaking changes
## Resources

[Commit Message Comparisons: Good VS Bad Commits](https://dev.to/kamleshsah_33/good-commit-vs-bad-commit-commit-message-comparisons-1ggp?ref=dailydev)