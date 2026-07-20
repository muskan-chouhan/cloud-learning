# Amazon CloudWatch

## What is Amazon CloudWatch?

Amazon CloudWatch is AWS's monitoring and observability service.

It continuously monitors AWS resources, collects metrics, generates alarms, and helps monitor the health and performance of applications and infrastructure.

---

# Why do we need CloudWatch?

Without CloudWatch:

- No centralized monitoring
- Difficult to detect issues
- Manual health checking
- No automatic alerts

With CloudWatch:

- Monitor AWS resources
- Visualize metrics using graphs
- Create alarms
- Receive notifications
- Monitor application health

---

# What can CloudWatch Monitor?

- EC2
- EBS
- RDS
- Load Balancer
- Lambda
- Auto Scaling
- Billing Metrics

---

# Metrics

Metrics are numerical values collected from AWS resources over time.

Examples:

- CPU Utilization
- Network In
- Network Out
- Disk Read Bytes
- Disk Write Bytes
- Status Check

---

# Namespace

A Namespace is a logical container used to organize metrics of AWS services.

Examples:

- AWS/EC2
- AWS/EBS
- AWS/RDS
- AWS/Lambda

---

# Dimension

A Dimension identifies the specific resource to which a metric belongs.

Example:

Metric:
CPUUtilization

Dimension:
InstanceId = i-xxxxxxxx

---

# Statistics

CloudWatch can display metrics using different statistics.

Examples:

- Average
- Maximum
- Minimum
- Sum
- Sample Count

Example:

CPU Values:

10%
20%
30%
40%

Average = 25%

---

# Alarms

CloudWatch Alarms monitor metrics and trigger actions when a defined threshold is crossed.

Example:

IF

CPUUtilization > 5%

THEN

Alarm

---

# Amazon SNS

CloudWatch uses Amazon SNS (Simple Notification Service) to send notifications.

Flow:

CloudWatch Alarm

↓

Amazon SNS

↓

Email Notification

---

# Dashboards

Dashboards provide a graphical view of monitored resources.

Example:

- CPU Utilization
- Network Traffic
- Disk Activity

All metrics can be viewed from a single dashboard.

---

# Logs

Logs store application and system events.

Examples:

- Application Errors
- User Login
- Server Restart
- HTTP Errors

Metrics represent numerical values, while Logs represent events.

---

# CloudWatch Agent

CloudWatch Agent is installed on EC2 instances to collect additional system metrics.

Examples:

- Memory Usage
- Disk Usage
- Running Processes

By default, CloudWatch collects basic metrics such as CPU and Network usage.

---

# Billing Alarm

Billing Alarm monitors AWS estimated charges.

Example:

If

Estimated Charges > $1

↓

CloudWatch Alarm

↓

SNS

↓

Email Notification

---

# Monitoring Flow

EC2

↓

CloudWatch Metrics

↓

CloudWatch Alarm

↓

Amazon SNS

↓

Email Notification

---

# Practical Performed

✅ Viewed EC2 Metrics

✅ Monitored CPU Utilization

✅ Created CloudWatch Alarm

✅ Created SNS Topic

✅ Confirmed Email Subscription

✅ Triggered Alarm using High CPU

✅ Received Email Notification

---

# Real World Use Cases

- Server Monitoring
- CPU Monitoring
- Infrastructure Health Monitoring
- Billing Alerts
- Production Monitoring

---

# Interview Questions

1. What is Amazon CloudWatch?

2. What is a Metric?

3. What is a Namespace?

4. What is a Dimension?

5. What is a CloudWatch Alarm?

6. What is Amazon SNS?

7. Difference between Metrics and Logs?

8. What is CloudWatch Agent?

9. What is a Billing Alarm?

10. How does CloudWatch send notifications?

---

# Notes

Amazon CloudWatch is AWS's monitoring service.

It collects metrics, visualizes performance, creates alarms, and sends notifications using Amazon SNS.

CloudWatch does not fix problems automatically; it detects issues and alerts administrators.