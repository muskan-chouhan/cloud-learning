# EC2 Launch Notes

## What is EC2?

Amazon EC2 (Elastic Compute Cloud) is an AWS service that provides virtual servers (instances) in the cloud.

---

## Instance Configuration

- Name: aws-learning-web-server
- AMI: Ubuntu Server 24.04 LTS
- Instance Type: t3.micro
- Storage: 8 GB (gp3)
- Key Pair: my-web-server-key.pem
- Security Group:
  - SSH (22)
  - HTTP (80)

---

## Steps Performed

- Launched Ubuntu EC2 instance
- Created SSH Key Pair
- Configured Security Group
- Connected using Browser-based EC2 Instance Connect
- Verified login using:

```bash
whoami
```

Output:

```text
ubuntu
```

- Connected using Git Bash (SSH)

```bash
ssh -i my-web-server-key.pem ubuntu@PUBLIC_IP
```

- Successfully logged in to Ubuntu server
- Logged out using:

```bash
exit
```

- Stopped EC2 instance after practice

---

## Important Concepts Learned

- EC2
- Instance
- AMI
- Ubuntu
- SSH
- Key Pair
- Public IP
- Security Group
- Browser Connect
- Git Bash SSH Login
- Ubuntu User vs IAM User

---

## Interview Notes

### What is EC2?

EC2 is an AWS service that provides scalable virtual machines in the cloud.

### Why is Public IP required?

The Public IP identifies the EC2 instance on the Internet so that SSH knows which server to connect to.

### Why is Key Pair required?

The private key proves the client's identity, and the server verifies it using the stored public key.

### Difference between IAM User and Ubuntu User

IAM User:
- Used to log in to the AWS Console.

Ubuntu User:
- Linux operating system user used after SSH login.

### Difference between Stop and Terminate

Stop:
- Instance can be started again.
- Data remains.

Terminate:
- Permanently deletes the EC2 instance.