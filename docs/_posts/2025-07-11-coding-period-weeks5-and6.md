---
title:  "Coding Period - Weeks 5 and 6"
date:   2025-07-11 03:52:01 +0300
categories: blog
permalink: /coding-period-week5-and6
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The current focus is to write test for the Robotics Application Manager project.
I spent the these two weeks reviewing the RAM project structure, writing tests, and improving the code through refactoring and reformatting.


### Work Done
- [X] Finish testing setup
- [X] Refactor and reformat some modules (Manager, Models, ...)
- [X] Write tests for some transitions in RAM
    - [X] `connect` transition
    - [X] `launch_world` transition

### Work to be Done
- [ ] Finish all transition tests for RAM
- [ ] Deploy a CI workflow for RAM tests


#### Notes
- Make sure to set the linter version in CI workflows to avoid inconsistencies


### Resources
- [pytest - Get Started](https://docs.pytest.org/en/stable/getting-started.html)
- [Pydantic Docs](https://docs.pydantic.dev/latest/)