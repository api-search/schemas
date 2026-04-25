---
description: A deployable component within a Choreo project. Components represent services, API proxies, web applications, scheduled jobs, manual triggers, event handlers, or webhooks.
layout: schema
name: Choreo Component
properties_list:
- description: Unique identifier for the component.
  name: id
  type: string
- description: Name of the component.
  name: name
  type: string
- description: Type of the component.
  name: type
  type: string
- description: Description of the component.
  name: description
  type: string
- description: Git repository URL for the component source code.
  name: repoUrl
  type: string
- description: Git branch used for builds.
  name: branch
  type: string
- description: Buildpack used for the component.
  name: buildpackId
  type: string
- description: Project identifier the component belongs to.
  name: projectId
  type: string
- description: Organization identifier.
  name: orgId
  type: string
- description: Current status of the component.
  name: status
  type: string
- description: Timestamp when the component was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-component.json
slug: choreo-component
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
title: Choreo Component
---
