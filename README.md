# AWS Organizations Governance Project

## Project Overview

This project demonstrates how to implement centralized governance across multiple AWS accounts using AWS Organizations and Service Control Policies (SCPs).

The objective of this project is to enforce security controls, restrict resource usage, and maintain governance across a multi-account AWS environment.

---

# Organization Structure

![Organization Structure](screenshots/01-ou-structure.png)

This screenshot shows the AWS Organization structure with multiple Organizational Units (OUs) such as Dev, Test, and Prod.

---

# Service Control Policies (SCP)

## 1. SCP Creation – Deny Large EC2 Instances

![SCP Deny Large EC2](screenshots/02-scp-deny-large-ec2.png)

This policy restricts launching large EC2 instances in child accounts.

---

## 2. EC2 Launch Denied (Validation)

![EC2 Launch Denied](screenshots/03-ec2-large-denied.png)

This screenshot verifies that launching restricted EC2 instance types is denied by the SCP.

---

## 3. CloudTrail Protection Policy

![CloudTrail Protection](screenshots/04-scp-cloudtrail-protection.png)

This policy prevents users from stopping logging or deleting CloudTrail.

---

## 4. Region Restriction Policy

![Region Restriction](screenshots/05-scp-region-restriction.png)

This SCP restricts resource creation outside the allowed AWS region.

---

# Policies Attached to Root

![All Policies](screenshots/06-all-policies.png)

This screenshot shows all Service Control Policies attached to the Root of the AWS Organization.

---

# Additional Policy Validation

![EC2 Deny Proof](screenshots/07-ec2-deny-proof.png.png)

This screenshot shows proof that the policy enforcement is working as expected.

---

# AWS Services Used

* AWS Organizations
* AWS IAM
* Amazon EC2
* AWS CloudTrail

---

# Key Learnings

* Multi-account governance using AWS Organizations
* Implementing security controls using SCPs
* Restricting AWS services and regions
* Protecting CloudTrail from unauthorized actions

---

# Conclusion

AWS Organizations and Service Control Policies provide centralized governance across multiple AWS accounts.

This project demonstrates how enterprises can enforce security policies, restrict resource usage, and maintain compliance in AWS environments.

---

⭐ This project is part of my AWS / DevOps learning journey.
