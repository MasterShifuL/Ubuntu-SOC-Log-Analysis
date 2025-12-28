# Day 02 Task – Brute Force Log Analysis

## Case Description
During routine monitoring of authentication logs, multiple failed SSH login attempts were observed within a short time window.
Such behavior can indicate either normal user mistakes (e.g., mistyped passwords) or early signs of a brute force attack.

This task focuses on analyzing Linux authentication logs to determine whether repeated failed login attempts constitute a potential brute force scenario.

## Objective
The goal of this task is to:
- Identify repeated authentication failures from log data
- Analyze frequency, source, and timing of failed login events
- Differentiate between user error and suspicious behavior
- Classify the activity from a SOC analyst perspective

## SOC Context
Brute force attacks against SSH services are among the most common threats faced by Linux servers.
Early detection through log analysis is critical to prevent account compromise and further lateral movement.

