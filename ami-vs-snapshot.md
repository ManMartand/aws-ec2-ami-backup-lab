# AMI vs Snapshot

## AMI

An AMI is a complete image used to launch an EC2 instance.  
It includes information such as root volume snapshot, launch permissions, and block device mapping.

## Snapshot

A snapshot is a backup of an EBS volume.  
It is mainly used to restore or create new EBS volumes.

## Simple Difference

- AMI is used to launch a new EC2 instance.
- Snapshot is used to restore or copy EBS volume data.

## Example

If I want to recreate a full EC2 server, I use an AMI.  
If I only want to restore a disk/volume, I use an EBS snapshot.
