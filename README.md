# 🧪 Wipro Selenium Automation

**From clicking buttons in a browser to validating APIs with a full BDD framework.**

*A complete record of a test automation learning journey — labs, a capstone project, and certifications.*

`Python` · `Selenium WebDriver` · `unittest` · `PyTest` · `Behave (BDD)` · `Robot Framework` · `Requests` · `JSON Schema` · `Allure`

---

## 🗺️ The Journey

This repo is organized the way the program was actually learned — start at the
UI, work down to test architecture, then out to APIs:

```
   UI Automation  ──▶  Test Frameworks  ──▶  BDD + APIs  ──▶  Robot Framework  ──▶  Capstone
     (M1)                (M2)                 (M3)              (M4)          (real framework)
```

| | |
|---|---|
| 🖱️ | **Started** with raw Selenium — locators, waits, alerts, frames |
| 🧱 | **Structured** it — unittest, PyTest, Page Object Model |
| 🥒 | **Made it readable** — Behave BDD, `Given/When/Then`, REST calls |
| 🤖 | **Went keyword-driven** — Robot Framework |
| 🚀 | **Shipped it** — a full API automation framework with schema validation and Allure reports |

---

## 📁 What's Inside

### 1️⃣ Lab Workbook — module-wise experiments

Each module folder has numbered assignments; each assignment has its own
README (problem → objective → approach → result), source code, and a
`screenshots/` folder as proof of execution.

| Module | What it covers | # Assignments |
|:--|:--|:--:|
| **M1 · Selenium Automation** | WebDriver, locators, XPath/CSS, navigation, alerts, frames & windows, actions, tables, waits, JS execution | 6 |
| **M2 · Unit Test Frameworks** | `unittest`, PyTest, Page Object Model | 3 |
| **M3 · BDD & REST Automation** | HTTP clients, API automation, Behave BDD | 3 |
| **M4 · Robot Framework** | Keyword-driven & data-driven testing | 2 |

### 2️⃣ Capstone Project — the framework that ties it together

**A production-style API test framework** — `requests` + Behave BDD + JSON
Schema contract validation + Allure reporting — tested against
[jsonplaceholder.typicode.com](https://jsonplaceholder.typicode.com/) with an
auth flow demoed against [automationexercise.com](https://automationexercise.com/api_list).

```gherkin
Feature: User Management API

  Scenario: Fetch a single user
    Given the API is available
    When I request user with id 2
    Then the response status should be 200
    And the response should match the "user" schema
```

- 🔁 Reusable HTTP client layer, DRY by design
- 📐 Schema validation — checks response *shape*, not just status codes
- 📊 Allure reports with full request/response payloads per step
- 🗂️ Data-driven from JSON/YAML — no hardcoded test data
- 🌍 One env var flips between dev/staging/prod

→ Full setup & run instructions: [`api-automation-framework/README.md`](2_Capstone_Project/api-automation-framework/README.md)
→ Write-up: [`Project_Report/`](2_Capstone_Project/Project_Report)

### 3️⃣ Certificates

Program completion certificates, included as PDFs.
