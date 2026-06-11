# Support Scenario: AMI Backup Before Change

## Scenario

A production EC2 instance needs configuration changes or patching.  
Before making the change, the support team creates an AMI backup.

## Why

If the change causes an issue, the team can launch a new EC2 instance from the AMI and reduce recovery time.

## Steps

1. Check EC2 instance status
2. Confirm application/server is stable
3. Create AMI from the instance
4. Add proper name and tags
5. Wait for AMI status to become available
6. Proceed with change activity
7. Use AMI for rollback if required

## Operational Benefit

- Faster recovery
- Safer change execution
- Better rollback planning
- Useful for production support and incident handling
