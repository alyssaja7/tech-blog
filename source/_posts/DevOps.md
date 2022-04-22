---
title: OCI - DevOps Overview
---
[Reference] (https://docs.oracle.com/en-us/iaas/Content/devops/using/devops_overview.htm)
## DevOps Concepts

### DevOps project
```
A logical grouping of DevOps resources needed to implement a CI/CD workflow. 
```
DevOps resources can be ***artifacts, build pipelines, deployment pipelines, external connections, triggers, and environments***.

### environment
```
A reference to the compute resources to which artifacts are deployed. 
```
An environment can be a reference to a Function application, a group of Compute instances, or a Container Engine for Kubernetes (OKE) cluster.

### instance group
```
A group of compute hosts. 
```
Each instance group can have compute hosts ***only from one region at a time***.

### artifact
```
A collection of binaries and deployment manifests that are delivered to the target deployment environment. 
```
DevOps artifacts can be ***a container image, an instance group deployment configuration, a Kubernetes manifest, or a generic artifact***. 
Artifacts can be hosted on OCI repositories: Container Registry and Artifact Registry.

### deployment configuration artifact
```
Defines the artifacts to be downloaded to the instance and the location where the artifacts have to be copied. 
```
The configuration file also specifies the sequence of commands for deployment.

### code repository
```
Private Git repositories hosted by the DevOps service. 
```
You can ***store, manage, and develop source code*** with the DevOps code repositories.

### external connection
```
Defines the authorization needed to connect to external repositories. 
```
DevOps supports connections to GitHub and GitLab external repositories.

### stage
```
A single step in the pipeline. 
```
The DevOps service includes ***predefined stages***, which are used in a build or deployment pipeline.

### build pipeline
```
Defines a set of stages for the build process: building, testing and compiling software artifacts, delivering artifacts to OCI repositories, and optionally triggering a deployment.
```

### build specification
Contains build steps and instructions that are run by the service managed build runner.

### deployment pipeline
```
A sequence of steps for deploying a set of artifacts to a target environment. 
```
A deployment pipeline contains stages that run sequentially or in parallel.

### rollback
```
A way to manage issues identified with the deployment, including releasing a previous successfully deployed version of the software.
```

### trigger
```
A DevOps resource to filter incoming events from a source code repository and trigger an action to start a build run on a matching incoming commit.
```
Trigger also refers to the deployment pipeline stage to trigger the start of a deployment.

### deployment
```
A single run of a deployment pipeline. 
```
A deployment contains the state of all the stages running in a deployment pipeline.

### work request
```
A way to track an asynchronous running task for a DevOps project.
```

### 3 Ways to Access DevOps
- Console (browser-based interface)
- Oracle Cloud Infrastructure CLI
- REST APIs

## Authentication & Authorization
***Each service in Oracle Cloud Infrastructure integrates with IAM for authentication and authorization, for all interfaces (the Console, SDK or CLI, and REST API).***
[Overview of Identity and Access Management] (https://docs.oracle.com/en-us/iaas/Content/Identity/Concepts/overview.htm#Overview_of_Oracle_Cloud_Infrastructure_Identity_and_Access_Management)
Objective: lets you control who has access to which specific cloud resources

### IAM Component
- Resource
- User
- Group
- Dynamic Group
- Network Source
- Compartment
- Tenancy
- Policy
- Home Region
- Federation

### You can write policies to control access to all of the services within Oralce Cloud Infrastructure
