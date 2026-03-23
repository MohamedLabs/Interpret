# 🔍 Interpret: Human-Centric Cloud Financial Intelligence

[![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)
[![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/features/actions)

**Interpret** is a "Cloud Translation Engine" designed to bridge the gap between complex cloud infrastructure and business-level financial clarity. While most systems focus on "Digital Transformation," **Interpret** does the reverse: it transforms "software noise" into actionable "human insight."

---

## 🧠 Project Philosophy

In modern cloud environments, we are often drowning in data but starving for meaning. Interpret is built on three pillars:

*   **Humanization:** Translating cryptic resource IDs (e.g., `t3.medium`) into relatable business terms (e.g., "Staging Environment").
*   **Contextualization:** Adding financial and temporal context to every cent spent.
*   **Proactivity:** Shifting from reactive billing alerts to story-driven financial intelligence.

---

## ⚠️ The Problem & ✅ The Solution

| The Problem | The Interpret Solution |
| :--- | :--- |
| **Knowledge Gap:** Cloud invoices are written for machines, not humans. | **Contextual Interpretation:** Maps technical resource costs to business units. |
| **Hidden Costs:** Difficulty in assigning costs to specific projects. | **Democratic Data:** Simple, low-cost S3 dashboard for non-technical stakeholders. |
| **Delayed Response:** Discovering overspending only after the bill arrives. | **Story-Driven Alerts:** Notifications that explain the *why* behind the spend. |

---

## 🏗 System Architecture

```mermaid
graph TD
    subgraph "AWS Account (Cost Source)"
        A[EC2, S3, RDS, etc.]
    end

    subgraph "Interpretation Engine (Serverless)"
        EB[EventBridge Scheduler]
        L[Lambda: Contextual Interpreter]
        CE[Cost Explorer API]
    end

    subgraph "Outputs & Notifications"
        S3[S3 Dashboard]
        SNS[SNS Topic]
        EM[Email/Slack Alerts]
    end

    A -- Generates Costs --> CE
    EB -- Triggers Weekly --> L
    L -- Queries Raw Data --> CE
    L -- Processes & Translates --> L
    L -- Uploads Dashboard --> S3
    L -- Publishes Alert --> SNS
    SNS -- Delivers --> EM

    style L fill:#f96,stroke:#333,stroke-width:2px
    style CE fill:#69c,stroke:#333,stroke-width:1px
    style EB fill:#bbf,stroke:#333,stroke-width:1px
    style S3 fill:#dfd,stroke:#333,stroke-width:1px
    style SNS fill:#fdd,stroke:#333,stroke-width:1px
```

---

## 🛠 Tech Stack (Enterprise-Grade)

The project leverages a modern, fully-automated stack built with an **Infrastructure as Code (IaC)** mindset.

*   **IaC:** [Terraform](https://www.terraform.io/) (Modular & Version Controlled)
*   **Compute:** [AWS Lambda](https://aws.amazon.com/lambda/) (Python 3.12 Runtime)
*   **Storage:** [Amazon S3](https://aws.amazon.com/s3/) (Static Website Hosting)
*   **Observability:** [AWS CloudWatch](https://aws.amazon.com/cloudwatch/) & Cost Explorer API
*   **Automation:** [GitHub Actions](https://github.com/features/actions) (CI/CD Pipeline)

---

## 🚀 Getting Started

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-repo/interpret.git
    ```
2.  **Infrastructure Deployment:**
    Ensure you have Terraform installed and AWS credentials configured.
3.  **CI/CD Setup:**
    Add your `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` to GitHub Secrets.
4.  **Deploy:**
    Push to the `main` branch to trigger the automated deployment.

---

## 📈 Value Proposition

Interpret demonstrates expertise in:
- **FinOps:** Effectively managing and interpreting cloud costs.
- **Serverless Architecture:** Building scalable, event-driven systems.
- **DevOps/SRE:** Implementing professional CI/CD and automation principles.

> Developed with ❤️ by **Mohamed Labs**
