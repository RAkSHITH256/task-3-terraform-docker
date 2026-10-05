# Task 3 - Infrastructure as Code with Terraform

## Objective

Provision a local Docker container using Terraform.

## Tools Used

- Terraform
- Docker
- Docker Provider
- Nginx

## Project Description

This project demonstrates Infrastructure as Code (IaC) using Terraform.

Terraform was used to:

1. Pull the Nginx Docker image.
2. Create an Nginx Docker container.
3. Configure port mapping.
4. Verify the running container.
5. Check Terraform state.
6. Destroy the infrastructure.

## Architecture

```text
Terraform
    |
    v
Docker Provider
    |
    v
Docker Engine
    |
    +---- nginx:latest
             |
             v
       terraform-nginx
             |
       Host: 8900
             |
       Container: 80
