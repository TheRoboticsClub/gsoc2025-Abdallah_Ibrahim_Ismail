---
title:  "Final Report - CI & Testing"
date:   2025-09-09 03:52:01 +0300
categories: blog
permalink: /final-report
toc_label: Table of Content
toc: true
sidebar:
  nav: "docs"
---


**Organization**: [JdeRobot](https://jderobot.github.io/)  
**Student**: Abdallah Ismail ([GitHub](https://github.com/Apolo151), [LinkedIn](https://linkedin.com/in/abdallah-ismail15))  
**Mentors**: Pedro Arias-Perez, Pawan Wadhwani, Miguel Fernandez
**GSoC Project Page**: [Robotics Academy: CI & Testing](https://summerofcode.withgoogle.com/programs/2025/projects/msXOO4mb)

---

Hello everyone,

This summer, I had the opportunity to contribute to [Robotics Academy](https://jderobot.github.io/RoboticsAcademy/) through the Google Summer of Code 2025 program. My project focused on establishing an automated testing framework for the Robotics Academy (RA), Robotics Infrastructure (RI), and Robotics Application Manager (RAM) repositories. 
My project proposal can be found [here](https://drive.google.com/file/d/1dFJHO139j73nkt_5qDKmCxGMMtfub-CU/view?usp=sharing).

### About me
I am a final-year Computer Science student at Ain Shams University, Egypt. My core experience and interests are in Software Development, Infrastructure Engineering, and Robotics. I enjoy the mix of rigorous research and building real products.

I am passionate about open-source and have contributed to various projects, but my contribution to JdeRobot has been the most significant and rewarding experience so far.

### About the Project
The primary goal of this project is to establish an automated testing framework for the Robotics Academy (RA), Robotics Infrastructure (RI), and Robotics Application Manager (RAM) repositories.

This framework includes a suite of unit and integration tests to verify functional correctness and ensure that the software remains maintainable and robust. 
 
Additionally, the project focuses on creating continuous integration (CI) pipelines, ensuring early detection of issues, and fostering a culture of quality and accountability across the projects.

---

### Contribution Summary

#### Step 1 : Creating and enforcing a style guide
The first step of the project involved creating and enforcing a style guide for the three repositories: RA, RI, and RAM. This was crucial to ensure code consistency and maintainability across the projects. 
I started by analyzing the existing codebases and identifying used programming languages and tools, then I created a comprehensive style guide that covered best practices, naming conventions, formatting rules, and other relevant guidelines.

Then conducted a survey within the JdeRobot community to gather feedback and ensure that the style guide met the needs of all contributors. After finalizing the style guide based on the feedback received, I set up automated tools to enforce the style guide, such as linters and formatters, and integrated these tools into the CI pipelines. 
This ensured that any code changes would be automatically checked for compliance with the style guide before being merged into the main branches.


#### Step 2 : Robotics Application Manager (RAM) Tests

The next step involved creating unit and integration tests for the Robotics Application Manager (RAM) repository. I started by quickly reviewing the existing codebase to identify critical components and functionalities that required testing.

The Robotics Application Manager (RAM) is an advanced manager for executing robotic applications. It operates as a state machine, managing the lifecycle of robotic applications from initialization to termination.

I created a suite of test cases covering all valid and invalid transitions between states, ensuring that the state machine behaved as expected in various scenarios. I also created GitHub Actions workflows to automate the execution of these tests whenever code changes were pushed to the repository. This ensured that any issues were detected early in the development process.


#### Step 3 : Robotics Infrastructure (RI) Tests

After completing the tests for RAM, I moved on to the Robotics Infrastructure (RI) repository. The RI repository provides essential services and tools that support the development and deployment of robotic applications.

The main focus was creating ROS2 launch tests for the **Launchers** that RI provides.

I first created tests for the main exercises that use Gazebo11 and ROS2 Humble. This involved setting up the test environments, writing launch test files, and validating the expected behaviors. After establishing this testing foundation, I then implemented additional tests for exercises that were newly migrated to use Gazebo Harmonic, ensuring compatibility with the latest simulation platform.

#### Step 4 : Robotics Academy (RA) Tests

Robotics Academy is the main project of JdeRobot. It utilizes the Robotics Infrastructure (RI) and Robotics Application Manager (RAM) to provide a comprehensive learning platform for robotics enthusiasts.

I started by reviewing the architecture of the RA project and its components, then created a testing plan for its frontend and backend.

- The frontend plan focuses on unit testing React-based components.
- The backend plan focuses on unit testing the different interfaces provided by RA.

I focused on creating tests for the most important HAL (Hardware Abstraction Layer) interfaces, including Camera, Lidar, and others.

Tests for other components are planned for future contributions.

---

### Demo Video

Here's a demonstration & visualization of some of the implemented tests for each of the projects:


---

### GitHub Contributions

Over the summer, I submitted a total of 13 pull requests across 3 repositories. These pull requests addressed 16 issues, and my contributions will be incorporated into the upcoming releases of JdeRobot’s Robotics-Academy.

| Pull Request | Solves Issue | Description | More |
|:------------:|:------------:|:-----------:|:----:|
| [Robotics Application Manager](https://github.com/JdeRobot/RoboticsApplicationManager)  |
| [#220](https://github.com/JdeRobot/RoboticsApplicationManager/pull/220), [#224](https://github.com/JdeRobot/RoboticsApplicationManager/pull/224), [#226](https://github.com/JdeRobot/RoboticsApplicationManager/pull/226)        | [#211](https://github.com/JdeRobot/RoboticsApplicationManager/issues/211),[#212](https://github.com/JdeRobot/RoboticsApplicationManager/issues/212), [#214](https://github.com/JdeRobot/RoboticsApplicationManager/issues/214)          | Enforce style guide in CI and enable branch protections | [Week 3 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week3), <br> [Week 4 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week4) |
| [#229](https://github.com/JdeRobot/RoboticsApplicationManager/pull/229)        | [#225](https://github.com/JdeRobot/RoboticsApplicationManager/issues/225)          | Implement finite state machine transitions tests, and add docstrings to source code| [Weeks 5&6 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week5-and6), <br> [Week 7 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week7) |
| [Robotics Infrastructure](https://github.com/JdeRobot/RoboticsInfrastructure) |
| [#522](https://github.com/JdeRobot/RoboticsInfrastructure/pull/522), [#528](https://github.com/JdeRobot/RoboticsInfrastructure/pull/528), [#529](https://github.com/JdeRobot/RoboticsInfrastructure/pull/529)         | [#513](https://github.com/JdeRobot/RoboticsInfrastructure/issues/513), [#514](https://github.com/JdeRobot/RoboticsInfrastructure/issues/514), [#516](https://github.com/JdeRobot/RoboticsInfrastructure/issues/516)        | Enforce style guide in CI, enable branch protections, and setup contributing docs | [Week 3 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week3), <br> [Week 4 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week4) |
| [#549](https://github.com/JdeRobot/RoboticsInfrastructure/pull/549) | [#515](https://github.com/JdeRobot/RoboticsInfrastructure/issues/515), [#546](https://github.com/JdeRobot/RoboticsInfrastructure/issues/546) | Implement RI ROS2 launch tests, and enforce them in CI| [Week 9 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week9), <br> [Week 10 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week10), <br> [Week 11 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week11) |
|[Robotics Academy](https://github.com/JdeRobot/RoboticsAcademy)  |
| [#3142](https://github.com/JdeRobot/RoboticsAcademy/pull/3142), [#3143](https://github.com/JdeRobot/RoboticsAcademy/pull/3143), [#3145](https://github.com/JdeRobot/RoboticsAcademy/pull/3145)        |  [#3109](https://github.com/JdeRobot/RoboticsAcademy/issues/3109),[#3110](https://github.com/JdeRobot/RoboticsAcademy/issues/3110), [#3112](https://github.com/JdeRobot/RoboticsAcademy/issues/3112)       | Setup Style Guide, and enforce it in CI using linters and formatters | [Week 2 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week2), <br> [Week 3 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week3), <br> [Week 4 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week4) |
| [#3233](https://github.com/JdeRobot/RoboticsAcademy/pull/3233), -        | [#3195](https://github.com/JdeRobot/RoboticsAcademy/issues/3195), [#3111](https://github.com/JdeRobot/RoboticsAcademy/issues/3111), [#3194](https://github.com/JdeRobot/RoboticsAcademy/issues/3194)       | Setup HAL interfaces tests, and add docstrings to RA interfaces | [Week 12 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week12), <br> [Week 13 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week13), <br> [Week 14 Blog](https://theroboticsclub.github.io/gsoc2025-Abdallah_Ibrahim_Ismail/coding-period-week14) |


### Future Work

The core goal of this project was to establish a solid foundation for automated testing and CI in the Robotics Academy, Robotics Infrastructure, and Robotics Application Manager repositories, to act as a core base for future contributions and extensions.

Each repository now has a comprehensive test setup and documentation, making the process of adding new tests and increasing code coverage much easier.

The very next area for improvement is implementing the frontend testing plan, as it was put on hold to wait for a current migration from JavaScript to TypeScript for the RA frontend.

---

### Conclusion

Participating in Google Summer of Code 2025 has been an incredibly rewarding journey. This project enhanced my technical expertise in ROS 2, testing, and CI. It also allowed me to work on something that delivers real, impactful value to a large open-source community.

Collaborating with the JdeRobot community has been a highlight of this experience. I gained valuable insights into open-source workflows, collaborative development, and designing solutions that scale for real-world users.

I would like to express my gratitude to Prof. José María Cañas and the JdeRobot admins for providing this opportunity. A special thanks to my mentors Pedro Arias Pérez, Pawan Wadhwani, and Miguel Fernandez for their valuable guidance, insightful feedback, and support throughout the project.
