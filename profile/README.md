# Proxylity LLC

[Proxylity](https://proxylity.com) was founded in 2025 by Lee Harding to drive innovation in network-software development and make building modern UDP services as easy as creating HTTP APIs. Today, Proxylity’s flagship product, **UDP Gateway**, is a fully managed service that connects your UDP traffic directly to AWS serverless backends—Lambda, Step Functions, Firehose, DynamoDB, S3, CloudWatch, and more—without managing any servers.

## Our Mission

> To drive innovation in network software development by eliminating the undifferentiated heavy lifting of UDP backends, so developers can focus on business logic and value-added features.

## Product: UDP Gateway

- **Serverless UDP Handling**  
  Receive and process UDP traffic entirely in your AWS account. Simply write a Lambda, route to Firehose, or push to your choice of services—no VMs, no containers, no servers.

- **Secure by Design**  
  Use your own AWS IAM policies, VPC endpoints, and IP/CIDR allowlists to control who can send UDP packets to your backends.

- **Pay-as-You-Go**  
  No upfront fees—pay only for the packets you send and the resources you consume. Charges appear directly on your AWS bill.

- **Ideal for**  
  - Online gaming workflows that require rapid iteration  
  - IoT telemetry scenarios where developer and deployment agility are key  
  - Enterprise services like Syslog, RADIUS, DNS requiring global/internet scale

- **Launch Date**  
  Publicly launched March 10, 2025 on Product Hunt.

## Examples Repository

Our [examples](https://github.com/proxylity/examples) repo demonstrates real-world UDP patterns and solutions, with full commentary on analogous problems you might face:

- **IoT Telemetry Pipelines**: Ingest device messages into Firehose and S3, iterating quickly on schema changes.  
- **Game Server Events**: Route game-client actions into Step Functions to spin up new workflows in seconds.  
- **Captive-Portal Workflows**: Show how a web-initiated Step Function can be completed by a subsequent UDP callback—common in captive WiFi networks.

Proxylity follows an **IaC-first** philosophy: we provide CloudFormation Custom Resources that let you declare your UDP endpoints alongside all other AWS infrastructure in a single YAML/JSON template. No imperative scripts—just deploy your stack and start sending packets.

## Getting Started

1. **Sign up**  
   - One-click with your existing AWS account—no forms, no bureaucracy, no spam. We don’t even capture your email or other PII.  
   - Free to start; only pay for what you use.

2. **Install via AWS Marketplace**  
   - Subscribe to [Proxylity UDP Gateway](https://aws.amazon.com/marketplace/pp/prodview-cpvl5wgt2yo2e?sr=0-1&ref_=beagle&applicationId=AWSMPContessa) in seconds. No hassles, no spam.  
   - Billing handled by AWS; appears on your regular AWS invoice.

3. **Explore our Examples**  
   ```bash
   git clone https://github.com/proxylity/examples.git
   cd examples
   # follow each directory’s README to deploy specific use cases
   ```
4. **Read the Docs**
   - Full API reference, CloudFormation details, and troubleshooting tips at docs.proxylity.com.

## Community & Support
- **Forums & Feedback**  
  Join the discussion on [Reddit](https://www.reddit.com/r/aws/comments/1j63zqv/handling_udp_traffic_in_aws_with_serverless), [Product Hunt](https://www.producthunt.com/products/proxylity-udp-gateway), and [Hacker News](https://news.ycombinator.com/) to share feedback and request new examples.

- **Contact**  
  For general questions, enterprise inquiries or custom integrations, email: support@proxylity.com.

Copyright 2025 Proxylity LLC. All rights reserved.
