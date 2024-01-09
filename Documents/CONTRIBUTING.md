# 贡献指南 Contributing Guide

ComikNet 团队非常欢迎来自任何人的贡献，遵守这份指南能帮助我们更快地审查您的代码。

The ComikNet team warmly welcomes contributions from anyone, and following this guide can help us review your code more efficiently.

一般来说，我们将 PRs (Pull Requests) 分为两类：**错误修复** 和 **功能实现**，它们在都拥有一些相同基础要求的前提下还有着不同的具体要求。

Generally, we categorize PRs (Pull Requests) into two types: Bug Fixes and Feature Implementations, both having some common foundational requirements, with specific additional requirements for each.

## 基础要求 Foundational Requirements

### 提交规范 Commit Standards

您的提交信息必须整洁且有意义。一般来说，我们会要求提交信息按照 [约定式提交](https://www.conventionalcommits.org/zh-hans) 的规范来书写。简单总结如下：

Your commit messages must be neat and meaningful. Generally, we require commit messages to follow the [Conventional Commits](https://www.conventionalcommits.org/en) standards. A brief summary is as follows:

- 每一类提交的工作描述应以 `feat`, `fix`, `chore`, `ci`, `docs`, `style`, `refactor` 等开头。  
  The description of each category of work should start with `feat`, `fix`, `chore`, `ci`, `docs`, `style`, `refactor`, etc.
  
  - 例如，你实现了一个 `foo` 方法，同时修复了两个错误: `woo` 和 `bar`，你的提交信息就应该是 `feat: add foo method; fixes: woo and bar bugs`。  
    For example, if you implemented a `foo` method and fixed two bugs: `woo` and `bar`, your commit message should be `feat: add foo method; fixes: woo and bar bugs`.
    
- 如果功能有破坏性更改，它应该被单独视作一类并在工作类描述后加 `!`。  
  If a feature involves breaking changes, it should be considered a separate category and marked with `!` after the work type description.
  
- 请使用英文。
  Please use English.

鼓励使用 GPG 签名的提交。如果您不知道怎么做，请参阅 [关于提交签名验证](https://docs.github.com/authentication/managing-commit-signature-verification/about-commit-signature-verification)。

Committing with a GPG signature is encouraged. If you don't know how to do this, refer to [About commit signature verification](https://docs.github.com/authentication/managing-commit-signature-verification/about-commit-signature-verification).

避免一个提交内有太多的更改，一个提交应专注于一类工作。但是，不要恶意分拆大量提交。

Avoid having too many changes in a single commit; a commit should focus on one type of work. However, do not maliciously split up into a large number of commits.

提交不能出现大量无关更改，例如您配置的自动格式化 (除非您确信原格式有误并得到允许)。

Commits should not contain a lot of unrelated changes, such as your personal auto-formatting configuration (unless you are certain that the original format is incorrect and have been permitted to change it).

### PR 规范 PR Standards

请按照项目提供的 PR 模板来填写 PR 信息。

Please fill in the PR information according to the PR template provided by the project.

您可以在工作未完成时就打开一个 PR 以便于我们审查您已经完成的工作并给出反馈。但是，请务必将 PR 的状态设置为 `Draft` 防止意外合并。

You can open a PR even if your work is not completed yet, so we can review the work you have done and provide feedback. However, please make sure to set the status of the PR to `Draft` to prevent accidental merges.

## 错误修复 Bug Fixes

**错误修复** 是指要修复一个现有功能的错误，或者是修复一个现有功能的不足之处。

**Bug Fixes** refer to correcting errors in an existing feature or addressing shortcomings of an existing feature.

错误修复的提交需要:

Submissions for bug fixes need to:

- 这个错误已经被证明不是功能的正常实现  
  Prove that the bug is not a normal implementation of the feature
  
- 如果是 Issue 等来源，请在工作描述符后加上 `#{Issue 编号}` (不要带上{})  
  If sourced from an Issue, etc., please add `#{Issue Number}` after the work descriptor (do not include {})

## 功能实现 Feature Implementation

**功能实现** 是指要实现一个新的功能，或者是对现有功能的重构。

**Feature Implementation** refers to the introduction of a new feature or the restructuring of an existing feature.
