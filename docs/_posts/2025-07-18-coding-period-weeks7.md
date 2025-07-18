---
title:  "Coding Period - Week 7"
date:   2025-07-18 03:52:01 +0300
categories: blog
permalink: /coding-period-week7
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

I finished writing tests for all core transitions in the Robotics Application Manager (RAM) project. This week also included refactoring some modules and deploying a CI workflow to run the RAM tests.


### Work Done

- [X] Finish tests for all core transitions in RAM
    - [X] `prepare_visualization` transition
    - [X] `run_application` transition
    - [X] `pause` & `resume` transitions
    - [X] `terminate` transitions
- [X] Refactor and reformat some modules (Linter, VNC Server, ...)
- [X] Deploy a CI workflow that runs RAM tests


#### Notes
- Make sure to set the linter version in CI workflows to avoid inconsistencies


### Resources
- [pytest - Get Started](https://docs.pytest.org/en/stable/getting-started.html)
- [Pydantic Docs](https://docs.pydantic.dev/latest/)
- [How to Generate PyTest Coverage Report](https://www.browserstack.com/guide/generate-pytest-code-coverage-report)