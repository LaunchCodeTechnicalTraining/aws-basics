---
title: "EC2 Private RDS"
date: 2022-05-05T13:50:01-05:00
draft: false
weight: 105
---

## Private `RDS` Connected to `EC2` with new `VPC`
1. Created a new private RDS
1. Created a new VPC with RDS rules
    1. Added new security rules for ports required
        1. Allow ssh on port 22
        1. Allow 80 for spring app
        1. allow port 5432 for RDS database
        1. allow 443 for https
1. Created new EC2 with VPC

## Resources Used
- `VPC`
- `RDS`
- `EC2`

### VPC

1. Two Availability Regions
    1. example: `us-east-1-a`
    1. example2: `us-west-1-a`
1. Four Subnets
    1. Two Public Subnets
        1. One Public Subnet for Each region
    1. Two Private Subnets
        1. One Private Subnet for Each region
### RDS

1. Private Subnet
    1. No public access
    1. Only Internal Private access
1. Security Groups
    1. One Security Group
        1. Inbound rules for requests
            1. IPV4 PostgreSQL (TCP) on port 5432
        1. CIDR block:
            1. 10.0.0.0/16
        1. Outbound Rules
            1. All traffic all ports everywhere all the time
### EC2

1. Subnets
    1. Subnets are either public or private
    1. Availability Zones
        1. us-east-1-a
1. Security Groups
    1. Security group with multiple rules
        1. Inbound and Outbound
        1. Inbound rules
            1. Port 443 for https
            1. Port 80 for default http
        1. Outbound rules
            1. All traffic all the time everywhere
