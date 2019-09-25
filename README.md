# AWS EC2 Automated Start / Stop

This template can be used to automatically start and stop EC2 instances based on a cron schedule.

### CRON statements

Cron statements must be valid for CloudWatch events. See AWS Documentation:

The statement shown in the (example config)[config/aws-ec2-start-stop.config.example] file does the following:

STARTS the EC2 instances at 8AM PST, MON-FRI
STOPS the EC2 instances at 7PM PST, MON-FRI

### Instances

Instance IDs should be passed as comma-separated string in the `pInstances` parameter:

`i-00000, i-00001, i-00002`

