# Steps Performed

- Reviewed authentication logs using:
  - sudo less /var/log/auth.log
- Filtered login events:
  - sudo grep "session opened" /var/log/auth.log
- Filtered sudo activity:
  - sudo grep "sudo" /var/log/auth.log
