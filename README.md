# AWS Observability Capstone Project

## Project Overview
A full observability layer for a three-tier AWS application using CloudWatch, X-Ray, EventBridge, and Lambda.

## Architecture
- **Web Tier:** EC2 + Application Load Balancer
- **App Tier:** ECS Fargate
- **Data Tier:** Amazon RDS MySQL

## What Was Built
- CloudWatch Agent on EC2 collecting CPU, memory, disk and web server logs
- Centralized CloudWatch Log Groups for all tiers
- Logs Insights query to detect 5xx error spikes
- 3 CloudWatch Alarms (CPU, Memory, Error Count)
- EventBridge rule triggering Lambda for auto-remediation
- SNS notifications for on-call alerts
- CloudWatch Dashboard with key metrics

## Screenshots
| Component | Screenshot |
|-----------|------------|
| CloudWatch Metrics | 01-cloudwatch-metrics.png |
| Log Groups | 02-log-groups.png |
| Logs Insights Query | 03-logs-insights-query.png |
| Alarms | 04-alarms.png |
| Dashboard | 05-dashboard.png |
| EventBridge Rule | 06-eventbridge-rule.png |
| Lambda Function | 07-lambda-function.png |
| EC2 Instance | 08-ec2-instance.png |

## AWS Services Used
- Amazon EC2
- Amazon CloudWatch
- AWS X-Ray
- Amazon EventBridge
- AWS Lambda
- Amazon SNS
- Amazon RDS

## Report
See `Capstone_Observability_Report.docx` for full write-up.
