---
title:  "Coding Period - Week 4"
date:   2025-06-27 03:52:01 +0300
categories: blog
permalink: /coding-period-week4
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The focus of this week was to finish enforcing the coding standards and practices within the JdeRobot community through deploying CI pipelines and guides for developers, and refactoring/reformatting existing to match the new standards.
Also, start planning for the second objective of writing tests for the RAM project.


### Work Done This Week
- [X] Enforce branch protections in all JdeRobot repositories
- [X] Deploy **Coding Style Guide**(https://github.com/JdeRobot/RoboticsAcademy/blob/humble-devel/docs/coding_style_guide.md)
- [X] Research Pre-commit hooks pros and cons
- [X] Finish IDE setup guide to enforce the **Coding Style Guide**
- [X] RAM repository
    - [X] Plan initial tests
- [X] RA repository
    - [X] Refactor existing code to match the new standards


#### Notes
- Make sure to set the linter version in CI workflows to avoid inconsistencies


### Resources
- [Pre-commit hooks](https://pre-commit.com/)
- [Black GitHub Actions Integration](https://black.readthedocs.io/en/stable/integrations/github_actions.html)