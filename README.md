# 🚀 AgilePilot

> A cloud-native, DevOps-integrated Scrum Master Assistant powered by AWS

AgilePilot is an automation-first solution designed to help Scrum teams manage retrospectives, assign action items, send timely reminders, and integrate effortlessly with CI/CD workflows like AWS CodePipeline.

It streamlines communication, accountability, and visibility — all from a single DevOps-native backend.

---

## 🎯 Problem It Solves

- Forgetting or losing track of action items from retros
- Manually creating Jira tickets after every sprint
- Chasing follow-ups via Slack or email
- Lack of connection between deployments and team process
- No post-deployment feedback or retros connected to CI/CD

---

## 🛠️ Built With

| Service          | Purpose                        |
|------------------|--------------------------------|
| **AWS Lambda**   | Core API & logic engine        |
| **DynamoDB**     | Storage for action items       |
| **API Gateway**  | REST entrypoint                |
| **CodePipeline** | CI/CD integration              |
| **SNS / SQS**    | Reminders and notifications    |
| **Slack API**    | Bot-based alerts/reminders     |
| **JIRA API**     | Auto-create and update tickets |

---

## ⚙️ Core Features

- ✅ Create & track retrospective action items
- ✅ Auto-generate Jira tickets
- ✅ Schedule Slack reminders via AWS
- ✅ Integrate with AWS CodePipeline
- 🚧 Sentiment analysis of retros (Upcoming)
- 🚧 Gamified contribution tracker (Upcoming)
- 🚧 Web dashboard for retros and leaderboards

---


## 🧱 Architecture Diagram

'''mermaid
flowchart TD
    A[User (Scrum Team)] -->|Message| B(Slack Bot)
    B --> C(API Gateway - AWS)
    C --> D[Lambda Functions]
    D --> E[DynamoDB (Action Items)]
    D --> F[JIRA API]
    D --> G[AWS SNS / EventBridge]
    G --> H[Slack Reminders]
    G --> I[CodePipeline Trigger]

    style A fill:#e3f2fd,stroke:#90caf9,stroke-width:2px
    style B fill:#fff3e0,stroke:#ffb74d,stroke-width:2px
    style C fill:#e8f5e9,stroke:#81c784,stroke-width:2px
    style D fill:#ede7f6,stroke:#9575cd,stroke-width:2px
    style E fill:#fce4ec,stroke:#f06292,stroke-width:2px
    style F fill:#f3e5f5,stroke:#ba68c8,stroke-width:2px
    style G fill:#e1f5fe,stroke:#4fc3f7,stroke-width:2px
    style H fill:#ffe0b2,stroke:#ff9800,stroke-width:2px
    style I fill:#d7ccc8,stroke:#8d6e63,stroke-width:2px

## 📦 Folder Structure (Planned)

