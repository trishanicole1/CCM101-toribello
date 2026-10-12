# Security Audit Report

## The Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving each user or program only the permissions needed to perform its tasks. This helps improve security by limiting the damage that could happen if an account is hacked or used incorrectly. For example, a user who only needs to view reports should not have permission to delete servers or modify important cloud resources.

## Attack Surface

The attack surface of a virtual machine includes all the possible points where an attacker could try to gain access. These include open ports, running services, applications, and user accounts. A larger attack surface creates more opportunities for attackers to exploit security weaknesses. To reduce risks, unnecessary ports should be closed, unused services should be disabled, and access should be properly controlled.

## Default Deny Policy

A Default Deny policy blocks all network traffic unless it is explicitly allowed by a security rule. This approach is safer than blocking known attackers one by one because new threats and unknown attackers may appear at any time. By allowing only necessary traffic, default deny reduces unauthorized access and helps protect cloud resources from potential attacks.
