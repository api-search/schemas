---
description: A build triggered for a Choreo component, representing the CI process of compiling and packaging component source code.
layout: schema
name: Choreo Build
properties_list:
- description: Unique identifier for the build.
  name: id
  type: string
- description: Component identifier this build belongs to.
  name: componentId
  type: string
- description: Current status of the build.
  name: status
  type: string
- description: Git commit hash the build was triggered from.
  name: commitHash
  type: string
- description: Git branch the build was triggered from.
  name: branch
  type: string
- description: Timestamp when the build was created.
  name: createdAt
  type: string
- description: Timestamp when the build completed.
  name: completedAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-build.json
slug: choreo-build
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
title: Choreo Build
---
