# AWS Technical Reference Guide: Core Services

This document serves as a structured technical reference for core Amazon Web Services (AWS) components, including Identity and Access Management (IAM), Elastic Compute Cloud (EC2), and Simple Storage Service (S3). It utilizes visual snapshots to illustrate key configurations and dashboard interfaces.

---

## Table of Contents
1. [Identity and Access Management (IAM)](#identity-and-access-management-iam)
2. [Elastic Compute Cloud (EC2)](#elastic-compute-cloud-ec2)
3. [Simple Storage Service (S3)](#simple-storage-service-s3)
4. [General Best Practices](#general-best-practices)

---

## Identity and Access Management (IAM)
IAM is the foundational security service used to manage access to AWS resources securely. It controls who is authenticated (signed in) and authorized (has permissions) to use resources.

### IAM Dashboard & Overview
The central hub for monitoring security status, managing users, and tracking credential usage.
![IAM Dashboard](iam-1.png)

### User and Group Management
*   **IAM Users:** Specific identities for persons or applications.
*   **IAM Groups:** Collections of users that share a common set of permissions.
![IAM Users](iam-2.png)

### Policies and Roles
*   **IAM Policies:** JSON documents that define permissions.
*   **IAM Roles:** Identities that can be "assumed" by trusted entities (like EC2 instances or Lambda functions).
![IAM Policies](iam-3.png)

---

## Elastic Compute Cloud (EC2)
Amazon EC2 provides scalable computing capacity in the AWS Cloud. It eliminates the need to invest in hardware upfront, allowing for faster development and deployment of applications.

### EC2 Management Console
The primary interface for launching, managing, and monitoring virtual servers.
![EC2 Dashboard](ec2-1.png)

### Instance Lifecycle
Managing running instances, selecting appropriate instance types (e.g., T3, M5), and monitoring health status.
![EC2 Instances](ec2-2.png)

### Connectivity and Security
*   **Security Groups:** Virtual firewalls that control inbound and outbound traffic.
*   **Key Pairs:** Secure login information for your instances.
![EC2 Security Groups](ec2-3.png)

---

## Simple Storage Service (S3)
Amazon S3 is an object storage service that offers industry-leading scalability, data availability, security, and performance.

### S3 Buckets
Containers for objects stored in S3. Every object is contained in a bucket.
![S3 Buckets](s3-1.png)

### Objects and Permissions
Managing individual data files (objects) and their associated metadata and Access Control Lists (ACLs).
![S3 Objects](s3-2.png)

### Management and Lifecycle Policies
Automating data transition and expiration to optimize costs over time.
![S3 Management](s3-3.png)

---

## General Best Practices
*   **Principle of Least Privilege:** Grant only the permissions required to perform a task.
*   **MFA (Multi-Factor Authentication):** Enable MFA for all users, especially the root account.
*   **Regular Audits:** Periodically review IAM permissions and S3 bucket access.
