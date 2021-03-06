# AWS ECS Cluster Terraform Module #

This Terraform module creates an AWS ECS cluster.

[![CircleCI](https://circleci.com/gh/cn-terraform/terraform-aws-ecs-cluster/tree/master.svg?style=svg)](https://circleci.com/gh/cn-terraform/terraform-aws-ecs-cluster/tree/master)
[![](https://img.shields.io/github/license/cn-terraform/terraform-aws-ecs-cluster)](https://github.com/cn-terraform/terraform-aws-ecs-cluster)
[![](https://img.shields.io/github/issues/cn-terraform/terraform-aws-ecs-cluster)](https://github.com/cn-terraform/terraform-aws-ecs-cluster)
[![](https://img.shields.io/github/issues-closed/cn-terraform/terraform-aws-ecs-cluster)](https://github.com/cn-terraform/terraform-aws-ecs-cluster)
[![](https://img.shields.io/github/languages/code-size/cn-terraform/terraform-aws-ecs-cluster)](https://github.com/cn-terraform/terraform-aws-ecs-cluster)
[![](https://img.shields.io/github/repo-size/cn-terraform/terraform-aws-ecs-cluster)](https://github.com/cn-terraform/terraform-aws-ecs-cluster)

## Usage

Check valid versions on:
* Github Releases: <https://github.com/cn-terraform/terraform-aws-ecs-cluster/releases>
* Terraform Module Registry: <https://registry.terraform.io/modules/cn-terraform/ecs-cluster/aws>

        module "ecs-cluster" {
            source  = "cn-terraform/ecs-cluster/aws"
            version = "1.0.2"
            name    = var.name_preffix
            profile = var.profile
            region  = var.region
        }

## Input values

* profile: AWS API key credentials to use.
* region: AWS Region where the infrastructure is hosted in.
* name: The name of the cluster (up to 255 letters, numbers, hyphens, and underscores).

## Output values

* aws_ecs_cluster_cluster_name: The name of the cluster.
* aws_ecs_cluster_cluster_id: The Amazon ID that identifies the cluster.
* aws_ecs_cluster_cluster_arn: The Amazon Resource Name (ARN) that identifies the cluster.

