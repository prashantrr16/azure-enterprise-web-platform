# Solution Overview

## Objective

Deploy two Windows Virtual Machines running NGINX behind an Azure Load Balancer.

## Architecture

- Azure Resource Group
- Virtual Network
- Azure Load Balancer
- VM01 (Primary NGINX Server)
- VM02 (Standby NGINX Server)
- Azure Function App
- VM Extension 

## Cost Optimization

VM02 remains deallocated during non-business hours.

Azure Function App automatically starts VM02 every morning using a timer trigger.

## Benefits

- High Availability
- Automated Operations
- Reduced Azure Compute Costs
- Infrastructure as Code
