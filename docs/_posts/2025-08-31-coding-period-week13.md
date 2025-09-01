---
title:  "Coding Period - Week 13"
date:   2025-08-31 03:52:01 +0300
categories: blog
permalink: /coding-period-week13
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The focus of this week was to implement the backend tests and improve in code documentation for the RoboticsAcademy Project.



**RoboticsAcademy Tests Structure**

```
tests/
├── conftest.py                 # Pytest configuration and fixtures
├── django/
│   ├── test_models.py          # Django model tests
│   └── test_views.py           # Django view tests
├── hal_interfaces/
│   ├── test_camera.py          # Camera interface tests
│   ├── test_motors.py          # Motors interface tests
│   └── test_laser.py           # Laser interface tests
├── gui_interfaces/
│   ├── test_threading_gui.py   # ThreadingGUI tests
│   └── test_measuring_gui.py   # MeasuringThreadingGUI tests
├── console_interfaces/
│   └── test_console.py         # Console interface tests
└── mocks/
    ├── mock_ros.py             # ROS mocks
    ├── mock_ros_messages.py    # ROS message mocks
    └── mock_websocket.py       # WebSocket mocks
```


### Work Done
- [X] Experiement with Django models and views tests
- [X] set up interfaces tests
- [X] add docstrings to interfaces code

### Remaining Work
- [X] Finalize interfaces tests
- [X] Create CI workflow to enforce tests

### Resources
- [Django Testing - Docs](https://docs.djangoproject.com/en/5.2/topics/testing/overview/)
- [PyTest Django - Docs](https://pytest-django.readthedocs.io/en/latest/)
- [Robotics Academy Architecture](https://github.com/JdeRobot/RoboticsAcademy/blob/humble-devel/docs/clientside.md)