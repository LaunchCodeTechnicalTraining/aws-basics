---
title: "Curriculum Outline"
date: 2022-05-04T13:45:41-05:00
draft: false
hidden: false
weight: 200
---

## Outline of AWS Curriculum
	- Goal of Class
		- Learning how to deploy an application to the cloud, not necessarily learning about AWS specifically
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
		- Creating new users
		- Creating new groups
	- EC2
		- Instance Types

## Final Project
	- MVC Application
		- Stretch Goal
			- Front end todo, API todo
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


## Questions ?
	- Exercises?
	- What do I want to give them? Having taught the Linux course what did they say they liked or learned the most from?
	- Really enjoyed the exercises, enjoyed the Q&A.
	- Source code repo or artifacts, requirements for infrastructure, paragraph? list? ec2? rds? s3? How is that outlined? Drawn diagram?
	- How to deliver the information as curriculum developer and teacher
	- Diagram to reflect infrastructure?
		- Potential Exercise


## Walkthrough Order
	- Basic EC2 Console + CLI
	- Smallest I can build for using the web console?
		- 2 or 3 POCs for only web console instructions for EC2 static, S3 Static, EC2 MVC
		- Then do CLIs for exact same things
	- Is end goal to deploy everything with CLI? Or to use some combination of CLI and console they are comfortable deploying basic things on their own
	- Company will move towards IAC
	- Maybe not everything needs CLI instructions? Bonus missions to use CLI to accomplish the same things they just did
	- 
