---
layout: post
title: Workflow Automation
subtitle: A Python Package
type: project
permalink: workflow-automation-project
---

The following is the README.md from my Workflow Automation project. The goal of the project is to maintain a single Python package where I can put scripts that help automate tasks I find myself doing often. For now it's only available on the Test PyPI repository. When it matures however, I may move it to the real PyPi repo. [Here's](https://github.com/joshortner/WorkflowAutomation) a link to the GitHub page.

---

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)

# Workflow Automation Package 

This package contains programs to automate some of the things I find myself doing often.

## Installation

Use the package manager pip to install workflow-automation package

```bash
pip install -i https://test.pypi.org/simple/ workflow-automation-pkg-joshortner
```

## cmake-man

cmake-man is a CLI program to manage CMake projects without having to hand-edit a CMakeLists.txt. Its based off of my personal experience using CMake. The functionality and project structure is defined below.

### Usage

Create a CMake Project

```bash
mkdir <project_name>
cd <project_name>
cmake-man --init --lang c
```

Project Structure:

```bash
C:/path/to/my_project
│   CMakeLists.txt
│
├───lib
└───src
    │   main.<lang>
    │   my_project.h
    │
    └───my_project
```

Build a CMake Project. This will add a "build" directory and generate files for the system's default compilation tools.

```bash
cmake-man --build
```
