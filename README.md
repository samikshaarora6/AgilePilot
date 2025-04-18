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

## 📦 Folder Structure (Planned)

