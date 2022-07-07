---
title: "Curriculum Outline"
date: 2022-05-04T13:45:41-05:00
draft: false
hidden: false
weight: 200
---

## Outline of AWS Curriculum

### EC2 Static
	- Web Console
	- CLI
### EC2 RDS
	- Web Console
		- Public RDS
		- Private RDS
	- CLI
		- Public RDS
		- Private RDS
### S3 to serve Static Files
	- Web Console
	- CLI

## Other Topics to Potentially Include:
	- IAM
		- IAM Policy Structure
		- MFA
		- Creating new users
		- Creating new groups
	- EC2
		- Instance Types

## Final Project
	- Full stack project deployed using console and CLI
		- Angular/React + Spring/.NET + Database
	- Completed using User Data for initialization Script
	- Project can be something created previously, LC101 assignment, previous LiftOff Graduate project

## EC2 First Walkthrough
	- Creating a new EC2
	- image AMI
	- Instance Type
	- Number of Instances
	- SSH Key Pair
	- VPC ID
	- Subnet ID
	- Security ID

	- Change Permissions on Created SSH
	- ssh -i path/to/keypair ubuntu@server-ip
	- Once inside of the instance, do what?

	- Recreate Steps for CLI

## EC2 Static Server Walkthrough
	- Create new EC2 using previously created subnets, security groups
	- Initialize Static File Server with User Data

	- Recreate Steps for CLI

## EC2 RDS Walkthrough
	- Create your first RDS database
	- Provide Subnet
	- Provide Security Group
	- Connect RDS to Existing EC2

## S3 Bucket Walkthrough
	- Create new S3 Bucket
	- secure copy files from local machine to s3 bucket as example
	- secure copy build artifcats to s3 bucket and initialize static website
