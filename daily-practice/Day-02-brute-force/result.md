# Day 02 Result – Brute Force Log Analysis

## Summary
Multiple failed SSH login attempts were detected during log review.
The activity was analyzed to determine whether it represented user error or a brute force pattern.

## Key Findings
- Repeated failed login attempts were observed.
- All attempts originated from the same source.
- Events occurred within a short time window.

## Analysis
WA single failed login attempt is common and typically caused by human error.
However, multiple failed login attempts originating from the same IP address within a short time window strongly suggest automated behavior.

Key indicators used in this analysis include source IP consistency, timestamp proximity, and attempt frequency.
The observed pattern aligns with common SSH brute force characteristics.


## Incident Classification
- Type: Potential SSH Brute Force Attempt
- Severity: Low (controlled lab environment)
- Confidence: Medium

## Analyst Reflection
SOC analysts must carefully distinguish between normal user mistakes and malicious activity.
Time correlation plays a crucial role in reducing false positives, as automated attacks generate login attempts at a speed unrealistic for human behavior.

## Recommended Response
In a production environment, the appropriate initial response would include temporary IP blocking and enhanced monitoring to prevent further unauthorized access attempts.


## Evidence
Screenshots are available in the `screenshots/` directory.

