---
title:  "Coding Period - Week 14"
date:   2025-09-07 03:52:01 +0300
categories: blog
permalink: /coding-period-week14
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
- [X] Implement tests for all HAL interfaces (Camera, Motors, Laser) -> [branch](https://github.com/JdeRobot/RoboticsAcademy/tree/backend_testing)
- [X] add docstrings to HAL interfaces code
- [ ] Create CI workflow to enforce interfaces tests


### Resources
- [Django Testing - Docs](https://docs.djangoproject.com/en/5.2/topics/testing/overview/)
- [PyTest Django - Docs](https://pytest-django.readthedocs.io/en/latest/)
- [Robotics Academy Architecture](https://github.com/JdeRobot/RoboticsAcademy/blob/humble-devel/docs/clientside.md)