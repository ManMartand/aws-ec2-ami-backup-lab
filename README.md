# AWS EC2 AMI Backup Lab

## Overview

This project demonstrates how to create an Amazon Machine Image (AMI) from an existing EC2 instance.  
An AMI can be used to back up an instance, create a reusable server image, launch similar instances faster, and support recovery during infrastructure issues.

## Objective

To create an AMI image from an EC2 instance using the AWS Management Console.

## Tools Used

- AWS EC2
- Amazon Machine Image (AMI)
- EBS Snapshot
- AWS Management Console

## Why AMI is Useful

In cloud operations and support, AMIs are useful for:

- Creating backup images of EC2 instances
- Rebuilding servers quickly
- Creating a standard/golden image for repeated deployments
- Supporting disaster recovery
- Reducing manual setup during incident recovery

## Steps Performed

1. Opened AWS Management Console
2. Navigated to EC2 service
3. Launched an EC2 instance
4. Selected the running EC2 instance
5. Opened **Actions → Image and templates → Create image**
6. Entered AMI name and description
7. Verified attached EBS volume details
8. Created the AMI
9. Confirmed successful AMI creation

## Support Scenario

Example scenario:

An application server is running on an EC2 instance. Before making configuration changes or patching activity, a support engineer creates an AMI backup. If the change fails, the team can launch a new instance from the AMI and restore service faster.

## Key Learning

- Understood how AMIs are created from EC2 instances
- Learned that AMI creation also creates snapshots of attached EBS volumes
- Practiced a basic backup and recovery workflow
- Understood how AMIs support server rebuild and operational continuity

## Interview Explanation

I created an AMI from an EC2 instance as part of an AWS backup and recovery lab. The purpose was to understand how support teams can create reusable server images before changes, patching, or risky configuration updates. The AMI can later be used to launch a new EC2 instance with the same base configuration, which helps in recovery and faster provisioning.

## Future Improvements

- Create AMI using AWS CLI
- Automate AMI creation using Lambda
- Add lifecycle cleanup for old AMIs and snapshots
- Use tags for environment, owner, and backup date
- Create a launch template using the AMI
