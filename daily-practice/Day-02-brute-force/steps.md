# Steps Performed – Brute Force Analysis

## 1. Event Generation (Controlled Environment)
To generate authentication failure events, multiple SSH login attempts were made to the local system using an incorrect password.
This was done intentionally on a personal lab machine to safely simulate real-world login failure scenarios.

## 2. Log Source Identification
The primary log source used for this analysis was:
- /var/log/auth.log

This file records authentication-related events such as login attempts, failures, and privilege usage.

## 3. Filtering Failed Authentication Events
Authentication failures were filtered using keyword-based searches to isolate relevant events:

- Failed SSH login attempts were identified using the "Failed password" keyword.
- Recent events were reviewed to focus on a short time window.

## 4. Pattern Analysis
Filtered log entries were analyzed to determine:
- Number of failed attempts
- Source IP address consistency
- Time interval between attempts

These factors were used to assess whether the activity followed a brute force pattern rather than isolated user mistakes.

## 5. Threshold Evaluation
A basic SOC detection threshold was applied:
- Multiple failed login attempts
- Same source IP
- Occurring within a short time frame

This threshold helps reduce false positives while still detecting suspicious behavior.

