---
title:  "Coding Period - Week 12"
date:   2025-08-22 03:52:01 +0300
categories: blog
permalink: /coding-period-week12
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---

The focus of this week was to fix issues with packages conflict to ensure Gazebo Harmonic is used correctly for related tests, and finalize the CI workflows for the RoboticsInfrastructure project.

Also, I finalized the plan for the backend tests for the RoboticsAcademy Repository.


#### Backend Testing Plan

The backend testing strategy covers Django models and views, hardware abstraction layer (HAL) interfaces, GUI and console interfaces.

- Django tests validate model creation, relationships, and API endpoints using isolated test data. 
- HAL interface tests use mocks to simulate ROS messages and hardware, ensuring correct data processing for camera, motors, and laser components. 
- GUI interface tests verify websocket communication and threading
- Console interface tests check stream redirection and cleanup. 

All tests should use mock objects to avoid altering the database or requiring simulators.

**Example Tests Structure**
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

- [X] RoboticsInfrastructure: Fix packages conflict
- [X] RoboticsInfrastructure: Update CI workflow for Gazebo Harmonic tests
- [X] RoboticsAcademy: Finalize backend testing plan


### Resources
- [aerostack2 Gazebo Installation](https://aerostack2.github.io/_03_aerial_platforms/_gazebo_simulation/index.html#installation)
- [Django Testing - Docs](https://docs.djangoproject.com/en/5.2/topics/testing/overview/)
- [Robotics Academy Architecture](https://github.com/JdeRobot/RoboticsAcademy/blob/humble-devel/docs/clientside.md)