# 📅 Day 9 — GitHub Actions (Automation Basics)

Today we learn how to **automate tasks on GitHub** using **GitHub Actions**.
Automation is widely used in real projects for testing, building, and deployments.

This skill is very valuable for:
- Internships
- Team projects
- Industry workflows (CI/CD basics)

---

## 🎯 Learning Objectives
By the end of Day 9, you will understand:
- What GitHub Actions are
- Why automation is important
- What workflows, jobs, and steps mean
- How to create a basic workflow

---

## 🤖 What is GitHub Actions?
GitHub Actions is a feature that allows you to **automate workflows** directly
inside your GitHub repository.

You can automatically:
- Run tests on every push
- Check code formatting
- Build projects
- Deploy applications

---

## ⚙️ Key Terms in GitHub Actions

### 1️⃣ Workflow
A workflow is an automated process.
It is defined using a **YAML (.yml)** file.

Workflows live inside:

---

### 2️⃣ Job
A job is a set of steps that run together.
A workflow can have one or more jobs.

---

### 3️⃣ Step
A step is a single task inside a job.
Example:
- Checkout code
- Run a command
- Print a message

---

### 4️⃣ Trigger
Triggers decide **when** the workflow runs.
Common triggers:
- push
- pull_request
- manual (workflow_dispatch)

---

## 🗂️ Folder Structure for Actions

---

## 🛠️ Create Your First GitHub Action (Basic Example)

Create a file:

Add this content:

```yml
name: Hello World Action

on: [push]

jobs:
  say-hello:
    runs-on: ubuntu-latest
    steps:
      - name: Print Hello
        run: echo "Hello from GitHub Actions!"
