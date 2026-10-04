# EC2 Server Observability and Monitoring Using Amazon CloudWatch

## 📌 Project Overview

This project demonstrates how Amazon CloudWatch can be used to monitor and observe an Amazon EC2 Linux server.

The solution collects system-level metrics and logs from an EC2 instance using the Amazon CloudWatch Agent. The collected information is visualized through a CloudWatch Dashboard, while a CloudWatch Alarm is used to detect high CPU utilization.

---

## 🎯 Problem Statement

EC2 servers require continuous monitoring to identify performance issues such as high CPU usage, memory utilization, disk usage, and abnormal network activity.

Without centralized monitoring, troubleshooting server issues can become difficult and time-consuming.

This project provides a centralized observability solution using Amazon CloudWatch.

---

## 🎯 Objectives

- Monitor EC2 server performance
- Collect CPU utilization metrics
- Monitor memory utilization
- Monitor disk utilization
- Monitor network activity
- Collect system logs
- Visualize metrics using a CloudWatch Dashboard
- Configure an alarm for high CPU utilization
- Provide centralized visibility for troubleshooting

---

## 🏗️ Architecture

```text
                Amazon EC2
              Amazon Linux
                    |
                    v
           CloudWatch Agent
              /          \
             /            \
        Metrics            Logs
           |                |
           v                v
   CloudWatch Metrics   CloudWatch Logs
           |
           v
   CloudWatch Dashboard
           |
           v
      CPU Alarm
