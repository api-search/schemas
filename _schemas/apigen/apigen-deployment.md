---
description: A deployment record representing an API deployed to a target environment.
layout: schema
name: APIGen Deployment
properties_list:
- description: Unique identifier for the deployment.
  name: id
  type: string
- description: ID of the deployed API.
  name: apiId
  type: string
- description: ID of the parent project.
  name: projectId
  type: string
- description: Target environment for the deployment.
  name: environment
  type: string
- description: Current status of the deployment.
  name: status
  type: string
- description: Live URL of the deployed API, available once deployment succeeds.
  name: url
  type:
  - string
  - 'null'
- description: Version of the API that was deployed.
  name: version
  type: string
- description: Cloud region where the API is deployed.
  name: region
  type: string
- description: Number of running instances.
  name: replicas
  type: integer
- description: Deployment log entries.
  name: logs
  type: array
- description: User ID of the person who initiated the deployment.
  name: deployedBy
  type: string
- description: Timestamp when the deployment was initiated.
  name: createdAt
  type: string
- description: Timestamp when the deployment record was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-deployment-schema.json
slug: apigen-deployment
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen Deployment
---
