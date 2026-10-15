# 🛡️ Enterprise Self-Healing Test Automation & Quality Engineering Framework

![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen?style=flat-square)
![Framework](https://img.shields.io/badge/Stack-Java%20%7C%20Selenium%20%7C%20Playwright%20%7C%20REST%20Assured-blue?style=flat-square)
![Self-Healing](https://img.shields.io/badge/Self--Healing-Healenium-orange?style=flat-square)
![Status](https://img.shields.io/badge/Project%20Status-Active%20%2F%20In--Progress-yellow?style=flat-square)

An enterprise-grade, resilient test automation framework demonstrating **self-healing UI locator strategies**, **API automation**, and **CI/CD Quality Gate integration**. Built to solve test flakiness, reduce script maintenance overhead, and enforce automated release readiness across dynamic enterprise applications.

> **📌 Portfolio Disclaimer:** This repository serves as an independent case study and practical reference architecture. Framework metrics and impact estimates noted below represent projected efficiency targets.

---

## 🎯 Key Capabilities & Architecture

* **Dynamic Self-Healing Locators:** Integrated **Healenium** and multi-attribute locator fallback strategies (Text, CSS, XPaths, Test-IDs) to auto-recover from UI/DOM changes at runtime without breaking build pipelines.
* **Dual UI Engine Support:** Core regression suite leverages **Java + Selenium WebDriver** and **Playwright**, demonstrating cross-browser stability and modern auto-waiting mechanisms.
* **Layered API Automation:** Backend API assertion engine powered by **REST Assured** and **Postman Mock Servers** to validate JSON schemas, HTTP status codes, and microservice payload contracts.
* **Data-Driven & Synthetic Test Data:** Driven by **TestNG `@DataProvider`** annotations and dynamic synthetic JSON payload generation to ensure environment independence.
* **CI/CD Quality Gate Integration:** Embedded test suites configured with strict **Entry/Exit criteria** and **Go/No-Go release readiness** status reporting for GitHub Actions / GitLab CI pipelines.

---

## 🛠️ Tech Stack & Dependencies

| Layer | Tools & Technologies |
| :--- | :--- |
| **Languages** | Java (JDK 17+), TypeScript / JavaScript |
| **UI Automation** | Selenium WebDriver, Playwright |
| **Self-Healing Engine** | Healenium (Web / Appium Wrapper) |
| **API Testing** | REST Assured, Postman Mock Servers |
| **Test Runner & BDD** | TestNG, Cucumber-JVM (Gherkin Syntax) |
| **Build & CI/CD** | Maven, GitHub Actions / GitLab CI/CD |
| **Reporting & RTM** | ExtentReports / Allure, Xray for Jira |

---

## 📂 Repository Structure

```text
├── .github/workflows/          # CI/CD pipeline triggers & quality gate configurations
├── src/
│   ├── main/java/
│   │   ├── drivers/            # WebDriver & Healenium wrapper initialization
│   │   ├── utils/              # Synthetic JSON generators, API helpers, & listeners
│   │   └── config/             # Environment & browser profile configurations
│   └── test/
│       ├── java/
│       │   ├── tests/          # TestNG UI & API test execution scripts
│       │   ├── pages/          # Page Object Model (POM) element locators & actions
│       │   └── stepdefs/       # Cucumber BDD step definitions
│       └── resources/
│           ├── features/       # BDD Gherkin scenario feature files
│           ├── testdata/       # JSON payload templates & schemas
│           └── testng.xml      # Execution suites (Smoke, Sanity, Regression)
├── healenium/                  # Healenium backend & tree-comparing service configs
├── pom.xml                     # Maven project dependencies & plugins
└── README.md
