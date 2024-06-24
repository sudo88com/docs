---
position: 3
title: "Detailed VPC CIDR block allocation"
tags: [infrastructure, terraform, terragrunt, aws, vpc, cidr]
---

### Detailed VPC CIDR Block Allocation

Our VPC CIDR blocks are allocated in a structured manner to ensure clarity and avoid conflicts across different environments. Below are the detailed allocations for development, pre-production, and production environments.

[https://github.com/sudo88com/aws-vpc-1](https://github.com/sudo88com/aws-vpc-1)

#### VPC CIDR Blocks

| Environment   | VPC CIDR Block  |
|---------------|-----------------|
| Development   | 148.3.0.0/16    |
| Pre-Production| 148.2.0.0/16    |
| Production    | 148.1.0.0/16    |

#### Subnet Allocations

For each VPC, the CIDR blocks are further divided into subnets to support various applications and services. Below is the detailed allocation from 148.0.0.0/16 to 165.0.0.0/16.

| CIDR Block      | Environment    | Notes                  |
|-----------------|----------------|------------------------|
| 148.0.0.0/16    | Reserved       | Future use             |
| 148.1.0.0/16    | Production     | Main production VPC    |
| 148.2.0.0/16    | Pre-Production | Testing and staging    |
| 148.3.0.0/16    | Development    | Development and testing|
| 148.4.0.0/16    | Reserved       | Future use             |
| 148.5.0.0/16    | Reserved       | Future use             |
| 148.6.0.0/16    | Reserved       | Future use             |
| 148.7.0.0/16    | Reserved       | Future use             |
| 148.8.0.0/16    | Reserved       | Future use             |
| 148.9.0.0/16    | Reserved       | Future use             |
| 148.10.0.0/16   | Reserved       | Future use             |
| 148.11.0.0/16   | Reserved       | Future use             |
| 148.12.0.0/16   | Reserved       | Future use             |
| 148.13.0.0/16   | Reserved       | Future use             |
| 148.14.0.0/16   | Reserved       | Future use             |
| 148.15.0.0/16   | Reserved       | Future use             |
| 148.16.0.0/16   | Reserved       | Future use             |
| 148.17.0.0/16   | Reserved       | Future use             |
| 148.18.0.0/16   | Reserved       | Future use             |
| 148.19.0.0/16   | Reserved       | Future use             |
| 148.20.0.0/16   | Reserved       | Future use             |
| 148.21.0.0/16   | Reserved       | Future use             |
| 148.22.0.0/16   | Reserved       | Future use             |
| 148.23.0.0/16   | Reserved       | Future use             |
| 148.24.0.0/16   | Reserved       | Future use             |
| 148.25.0.0/16   | Reserved       | Future use             |
| 148.26.0.0/16   | Reserved       | Future use             |
| 148.27.0.0/16   | Reserved       | Future use             |
| 148.28.0.0/16   | Reserved       | Future use             |
| 148.29.0.0/16   | Reserved       | Future use             |
| 148.30.0.0/16   | Reserved       | Future use             |
| 148.31.0.0/16   | Reserved       | Future use             |
| 148.32.0.0/16   | Reserved       | Future use             |
| 148.33.0.0/16   | Reserved       | Future use             |
| 148.34.0.0/16   | Reserved       | Future use             |
| 148.35.0.0/16   | Reserved       | Future use             |
| 148.36.0.0/16   | Reserved       | Future use             |
| 148.37.0.0/16   | Reserved       | Future use             |
| 148.38.0.0/16   | Reserved       | Future use             |
| 148.39.0.0/16   | Reserved       | Future use             |
| 148.40.0.0/16   | Reserved       | Future use             |
| 148.41.0.0/16   | Reserved       | Future use             |
| 148.42.0.0/16   | Reserved       | Future use             |
| 148.43.0.0/16   | Reserved       | Future use             |
| 148.44.0.0/16   | Reserved       | Future use             |
| 148.45.0.0/16   | Reserved       | Future use             |
| 148.46.0.0/16   | Reserved       | Future use             |
| 148.47.0.0/16   | Reserved       | Future use             |
| 148.48.0.0/16   | Reserved       | Future use             |
| 148.49.0.0/16   | Reserved       | Future use             |
| 148.50.0.0/16   | Reserved       | Future use             |
| 148.51.0.0/16   | Reserved       | Future use             |
| 148.52.0.0/16   | Reserved       | Future use             |
| 148.53.0.0/16   | Reserved       | Future use             |
| 148.54.0.0/16   | Reserved       | Future use             |
| 148.55.0.0/16   | Reserved       | Future use             |
| 148.56.0.0/16   | Reserved       | Future use             |
| 148.57.0.0/16   | Reserved       | Future use             |
| 148.58.0.0/16   | Reserved       | Future use             |
| 148.59.0.0/16   | Reserved       | Future use             |
| 148.60.0.0/16   | Reserved       | Future use             |
| 148.61.0.0/16   | Reserved       | Future use             |
| 148.62.0.0/16   | Reserved       | Future use             |
| 148.63.0.0/16   | Reserved       | Future use             |
| 148.64.0.0/16   | Reserved       | Future use             |
| 148.65.0.0/16   | Reserved       | Future use             |
