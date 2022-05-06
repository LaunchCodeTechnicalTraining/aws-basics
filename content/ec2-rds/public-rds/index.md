---
title: "Public RDS"
date: 2022-05-05T13:50:01-05:00
draft: false
weight: 100
originalAuthor: <no value> # to be set by page creator
originalAuthorGitHub: <no value> # to be set by page creator
reviewer: # to be set by the page reviewer
reviewerGitHub: # to be set by the page reviewer
lastEditor: # update any time edits are made after review
lastEditorGitHub: # update any time edits are made after review
lastMod: # UPDATE ANY TIME CHANGES ARE MADE
---

## AWS EC2 RDS Deployment Notes

### RDS

Creation Method: Easy Create 
1. database identifier: `database-1`
1. Recommended best practices
1. Some options can be changed after creation

Configuartion:
1. Engine Type: `PostgreSQL 13.4-R1`
1. DB Instance Size: `Free tier`
1. Db Instance idenfitifer: `Name of database`
1. Master Username: `username`

Instance Configuartion:
1. EC2 Instance Type: `db.t3.micro`

Storage:
1. Storage Type: `General Purpose SSD (gp2)`
1. Allocated Storage: `20 (default minimum)`
1. Storage Autoscaling: `Disabled`
1. Maximum Threshhold: `Removed when disabling Storage Autoscaling`

Connectivity:
1. VPC: 
1. Subnet Group:
1. Public Access: `No is the default setting`
1. VPC Security Group: Created new: `rds-public-access`
1. Availability Zone: `us-east-1a`
1. Database port: `5432`

Database Options:
1. initial database name: `students`
1. db param group: `default.postgres13`

## Content Links

{{% children %}}