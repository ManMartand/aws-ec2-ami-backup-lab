# Create AMI Using AWS CLI

## Command

```bash
aws ec2 create-image \
  --instance-id i-xxxxxxxxxxxxxxxxx \
  --name "webserver-backup-ami" \
  --description "AMI backup before patching activity" \
  --no-reboot
