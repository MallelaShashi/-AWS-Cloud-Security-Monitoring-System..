
# AWS Cloud Security Monitoring System

## Overview

This project is a cloud security monitoring system built using AWS services.
It helps monitor suspicious activities, track cloud events, and generate security alerts in real time.

---

## Features

- Real-time monitoring
- CloudTrail logging
- IAM activity tracking
- SNS notifications
- Security event alerts

---


## AWS Services Used

| Service | Purpose |
|----------|----------|
| Amazon EC2 | Hosted the OWASP Juice Shop vulnerable web application |
| AWS CloudTrail | Captured and recorded AWS account activity and API logs |
| Amazon GuardDuty | Detected suspicious activities and potential security threats |
| Amazon CloudWatch | Monitored logs, metrics, and security-related events |
| Amazon SNS | Sent real-time email alert notifications |
| OWASP Juice Shop | Simulated a vulnerable web application for security testing |
---

## Architecture

Add architecture diagram here.

---

## Workflow

## Workflow

```text
OWASP Juice Shop Hosted on EC2
                ↓
      User Activities & Requests
                ↓
        AWS CloudTrail Logs
                ↓
      Amazon GuardDuty Analysis
                ↓
    Suspicious Activity Detection
                ↓
         CloudWatch Monitoring
                ↓
         Amazon SNS Alerts
                ↓
      Email Notification to Admin
```

### Step-by-Step Explanation

1. OWASP Juice Shop is deployed on an AWS EC2 instance to simulate a vulnerable web application environment.

2. Users interact with the application, generating AWS account activities and security-related events.

3. AWS CloudTrail records API calls, account activity, and security logs from the AWS environment.

4. Amazon GuardDuty continuously analyzes CloudTrail logs and detects suspicious or malicious behavior such as:
   - Unauthorized access attempts
   - Reconnaissance activities
   - Suspicious API calls
   - Credential compromise indicators

5. Amazon CloudWatch monitors logs and security events generated within the environment.

6. When suspicious activity is identified, Amazon SNS sends real-time alert notifications to the administrator through email.

7. The administrator reviews alerts and takes necessary security actions to protect cloud resources.

## Security Use Cases

- Unauthorized login detection
- Root account usage alerts
- IAM policy monitoring

---


---

## Author
Seshagiri Mallela
