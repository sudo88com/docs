---
title: Subnets Implementation
tags: [infrastructure, terraform, terragrunt, aws, subnet, public, private]
---

Our VPC design includes both public and private subnets to segregate resources based on their accessibility requirements. Below are the detailed configurations for each environment, showing the VPC CIDR block allocations and subnet details.

[https://github.com/sudo88com/aws-vpc-1](https://github.com/sudo88com/aws-vpc-1)

#### VPC CIDR Blocks

| Environment   | VPC CIDR Block  |
|---------------|-----------------|
| Development   | 148.3.0.0/16    |
| Pre-Production| 148.2.0.0/16    |
| Production    | 148.1.0.0/16    |

#### Subnet Details

##### Development Environment

| Subnet Name                     | Subnet ID             | VPC ID              | Subnet CIDR Block | Availability Zone | Public | Private |
|---------------------------------|-----------------------|---------------------|-------------------|-------------------|--------|---------|
| default-dev-public-ap-south-1c  | subnet-026d786e86ca77434 | vpc-0d1e013ef4f71b105 | 148.3.103.0/24    | ap-south-1c      | Yes    | No      |
| default-dev-public-ap-south-1b  | subnet-003a307a75736bcf4 | vpc-0d1e013ef4f71b105 | 148.3.102.0/24    | ap-south-1b      | Yes    | No      |
| default-dev-public-ap-south-1a  | subnet-0397fe8ee83cd6ae5 | vpc-0d1e013ef4f71b105 | 148.3.101.0/24    | ap-south-1a      | Yes    | No      |
| default-dev-private-ap-south-1c | subnet-049bb40c3973f9700 | vpc-0d1e013ef4f71b105 | 148.3.3.0/24      | ap-south-1c      | No     | Yes     |
| default-dev-private-ap-south-1b | subnet-0f5d69d82732a87a6 | vpc-0d1e013ef4f71b105 | 148.3.2.0/24      | ap-south-1b      | No     | Yes     |
| default-dev-private-ap-south-1a | subnet-012602fa27576e056 | vpc-0d1e013ef4f71b105 | 148.3.1.0/24      | ap-south-1a      | No     | Yes     |

##### Pre-Production Environment

| Subnet Name                     | Subnet ID             | VPC ID              | Subnet CIDR Block | Availability Zone | Public | Private |
|---------------------------------|-----------------------|---------------------|-------------------|-------------------|--------|---------|
| default-pre-public-ap-south-1c  | subnet-0f6456269279e3d98 | vpc-0cebe69dde485d9e7 | 148.2.103.0/24    | ap-south-1c      | Yes    | No      |
| default-pre-public-ap-south-1b  | subnet-01d4efff423833af4 | vpc-0cebe69dde485d9e7 | 148.2.102.0/24    | ap-south-1b      | Yes    | No      |
| default-pre-public-ap-south-1a  | subnet-003b8e58347dc8dd0 | vpc-0cebe69dde485d9e7 | 148.2.101.0/24    | ap-south-1a      | Yes    | No      |
| default-pre-private-ap-south-1c | subnet-087fd7913eed1fca5 | vpc-0cebe69dde485d9e7 | 148.2.3.0/24      | ap-south-1c      | No     | Yes     |
| default-pre-private-ap-south-1b | subnet-09218542619261678 | vpc-0cebe69dde485d9e7 | 148.2.2.0/24      | ap-south-1b      | No     | Yes     |
| default-pre-private-ap-south-1a | subnet-067d65b616061a6d1 | vpc-0cebe69dde485d9e7 | 148.2.1.0/24      | ap-south-1a      | No     | Yes     |

##### Production Environment

| Subnet Name                     | Subnet ID             | VPC ID              | Subnet CIDR Block | Availability Zone | Public | Private |
|---------------------------------|-----------------------|---------------------|-------------------|-------------------|--------|---------|
| default-prod-public-ap-south-1c | subnet-05b1a5956edf65a80 | vpc-096eb7e720761963a | 148.1.103.0/24    | ap-south-1c      | Yes    | No      |
| default-prod-public-ap-south-1b | subnet-0a10ad32692ad209d | vpc-096eb7e720761963a | 148.1.102.0/24    | ap-south-1b      | Yes    | No      |
| default-prod-public-ap-south-1a | subnet-0ab5311f9feac9ed2 | vpc-096eb7e720761963a | 148.1.101.0/24    | ap-south-1a      | Yes    | No      |
| default-prod-private-ap-south-1c | subnet-0214b252363fbacd9 | vpc-096eb7e720761963a | 148.1.3.0/24      | ap-south-1c      | No     | Yes     |
| default-prod-private-ap-south-1b | subnet-0ae5b072660a08b6a | vpc-096eb7e720761963a | 148.1.2.0/24      | ap-south-1b      | No     | Yes     |
| default-prod-private-ap-south-1a | subnet-04da60d9a574b0277 | vpc-096eb7e720761963a | 148.1.1.0/24      | ap-south-1a      | No     | Yes     |

This document provides an overview of our VPC CIDR block allocations and the design and implementation of public and private subnets across different environments.
