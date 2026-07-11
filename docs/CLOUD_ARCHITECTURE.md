# Cloud Architecture

## Design objective

Build a low-cost, secure pilot that can verify waste transactions in Abuja, then scale only after repeat demand and reliable operations are demonstrated.

## Core workloads

1. Public website and low-bandwidth web application.
2. Identity and role-based access for customers, collectors, operators and partners.
3. Pickup request and dispatch workflow.
4. Evidence upload for images, weight records and supporting documents.
5. Settlement and incentive records.
6. Notifications and asynchronous jobs.
7. AI-assisted prioritisation, anomaly review and forecasting.
8. Analytics, audit logs and recovery reporting.
9. Encrypted backups, monitoring and incident response.

## Logical architecture

```text
Users
  -> CDN / WAF / rate limiting
  -> Web application
  -> API and identity
  -> workflow and queue
  -> relational operational database
  -> object storage for evidence
  -> AI inference and model monitoring
  -> analytics and partner reporting
  -> logs, alerts, backups and security controls
```

## AWS workload mapping

| Capability | Proposed AWS service |
|---|---|
| DNS, CDN and edge security | Route 53, CloudFront, AWS WAF, Shield Standard |
| Static web application | S3 or Amplify Hosting |
| API | API Gateway and Lambda |
| Authentication | Amazon Cognito |
| Operational database | Amazon RDS for PostgreSQL |
| Evidence storage | Amazon S3 with lifecycle policies |
| Background jobs | Amazon SQS and EventBridge |
| AI | Amazon Bedrock and/or SageMaker |
| Analytics | Athena, Glue and QuickSight |
| Monitoring | CloudWatch, CloudTrail and GuardDuty |
| Secrets and encryption | Secrets Manager and KMS |

## Microsoft Azure workload mapping

| Capability | Proposed Azure service |
|---|---|
| DNS, CDN and edge security | Azure DNS, Front Door and Web Application Firewall |
| Static web application | Azure Static Web Apps |
| API | Azure Functions and API Management |
| Authentication | Microsoft Entra External ID |
| Operational database | Azure Database for PostgreSQL |
| Evidence storage | Azure Blob Storage |
| Background jobs | Service Bus and Event Grid |
| AI | Azure AI Foundry and Azure Machine Learning |
| Analytics | Data Factory, Synapse or Fabric and Power BI |
| Monitoring | Azure Monitor, Application Insights and Defender for Cloud |
| Secrets and encryption | Key Vault |

## Cloudflare workload mapping

| Capability | Proposed Cloudflare service |
|---|---|
| DNS, CDN and edge security | Cloudflare DNS, CDN, WAF, DDoS and Bot protection |
| Static web application | Cloudflare Pages |
| API | Cloudflare Workers |
| Authentication protection | Turnstile and Access where appropriate |
| Operational database | D1 |
| Evidence storage | R2 |
| Background jobs | Queues, Workflows and Cron Triggers |
| AI | Workers AI and Vectorize |
| Stateful coordination | Durable Objects |
| Monitoring | Workers Analytics and Logpush |
| Team access | Zero Trust |

## Architecture principles

- Portable data model and open standards.
- Separate operational records from analytics and model features.
- Do not place sensitive personal data in public model prompts.
- Store original evidence separately from derived AI features.
- Enforce role-based access and least privilege.
- Retain manual override and decision history.
- Measure performance, cost and operational reliability before expanding.
