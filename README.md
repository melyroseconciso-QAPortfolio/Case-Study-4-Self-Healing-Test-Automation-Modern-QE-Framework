# 🛡️ Enterprise Self-Healing Test Automation & Quality Engineering Framework (AI-Assisted PoC)

![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen?style=flat-square)
![Framework](https://img.shields.io/badge/Stack-Java%20%7C%20Selenium%20%7C%20Playwright%20%7C%20REST%20Assured-blue?style=flat-square)
![Self-Healing](https://img.shields.io/badge/Self--Healing-Healenium-orange?style=flat-square)
![Project Type](https://img.shields.io/badge/Type-AI--Assisted%20Independent%20Study-purple?style=flat-square)

An independent, AI-assisted proof-of-concept framework exploring **self-healing UI locator strategies**, **API automation**, and **CI/CD Quality Gate integration**. This project was developed with AI assistance to evaluate methods for mitigating test flakiness, reducing maintenance overhead, and structuring automated release readiness across dynamic enterprise applications.

> **📌 Disclaimer & Transparency Note:** This repository is an independent case study and reference architecture developed with AI assistance. It serves to demonstrate technical exploration, prompt engineering integration, and quality framework design. Metrics and impact estimates noted are projected conceptual targets rather than measured production outcomes.

---

## 🎯 Key Capabilities & Architecture

* **AI-Assisted Design & Architecture:** Framework scaffolding, Gherkin scenario generation, and script structures were co-developed and refined using generative AI tools.
* **Dynamic Self-Healing Locators:** Integrated **Healenium** and multi-attribute locator fallback strategies (Text, CSS, XPaths, Test-IDs) to auto-recover from simulated UI/DOM changes at runtime.
* **Dual UI Engine Support:** Explores core regression suites leveraging **Java + Selenium WebDriver** and **Playwright** for cross-browser stability.
* **Layered API Automation:** Backend API assertion engine powered by **REST Assured** and mock servers to validate JSON schemas and payload contracts.
* **CI/CD Quality Gate Integration:** Configured with strict **Entry/Exit criteria** and **Go/No-Go release readiness** status reporting for pipeline execution.

---

## 🛠️ Tech Stack & Dependencies

| Layer | Tools & Technologies |
| :--- | :--- |
| **Languages** | Java (JDK 17+), TypeScript / JavaScript |
| **UI Automation** | Selenium WebDriver, Playwright |
| **Self-Healing Engine** | Healenium (Web / Appium Wrapper) |
| **API Testing** | REST Assured, Postman Mock Servers |
| **Test Runner & BDD** | TestNG, Cucumber-JVM (Gherkin Syntax) |
| **Build & AI Support** | Maven, GitHub Actions, LLM-Assisted Scripting |
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
