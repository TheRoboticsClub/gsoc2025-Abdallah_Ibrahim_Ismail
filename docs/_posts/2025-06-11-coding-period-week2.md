---
title:  "Coding Period - Week 2"
date:   2025-06-11 03:52:01 +0300
categories: blog
permalink: /coding-period-week2
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The focus of this week was to finalize the coding standards and practices within the JdeRobot community through more research and community surveys, and start enforcing these rules through developer guides and CI pipelines.


### Work Done This Week
- [X] Conduct community survey about Branch Protections
	- [X] research all common branch protections
    - [X] check main branches in main JdeRobot repositories
- [X] Finish the **Coding Style Guide**
	- [X] Add details for XML and YAML
- [ ] Finish IDE setup guide to enforce the **Coding Style Guide**
- [ ] Implement basic linting CI workflows for common languages
    - [ ] Finish Python linting CI workflow in RA repository
	- [ ] Setup a Javascript/JSX linting workflow in RA repository
- [ ] Finish **Setup ROS2 Package Guide**
	- [ ] list all common practices (compiler flags, linting, testing)


### Next Week Plan
- [ ] Setup final CI pipelines for all repositories

### Resources
- [GitHub Docs - About protected branches](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches)
- [GitHub Docs - About rulesets](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/about-rulesets)
- [Getting Started with ESlint](https://eslint.org/docs/latest/use/getting-started)
- [Using Black with other tools](https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html)