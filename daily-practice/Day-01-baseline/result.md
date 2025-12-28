# Day 01 Result – Baseline Observation

## Log Source
- /var/log/auth.log

## Normal Activity Observed
- User login activity occurred during normal working hours.
- All sudo commands were executed by the expected user (myself).
- No authentication errors or suspicious messages were observed.

## Time Pattern
- Login and privilege usage aligned with regular daily usage patterns.

## SOC Note
This baseline confirms that current authentication behavior is normal.
Future deviations from this pattern may indicate suspicious or unauthorized activity.

## Evidence
Screenshots of authentication logs and command outputs are available in the `screenshots/` directory.

## Analyst Reflection
At this stage, no security incident was identified.
However, establishing this baseline is critical to avoid false positives and unnecessary escalation in future analysis.
