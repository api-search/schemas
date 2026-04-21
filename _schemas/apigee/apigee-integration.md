---
description: A version of an integration containing the complete configuration including triggers, tasks, and parameters for automating workflows within Google Cloud.
layout: schema
name: Apigee Integration Version
properties_list:
- description: Output only. Resource name of the version.
  name: name
  type: string
- description: Description of the integration version.
  name: description
  type: string
- description: List of task configurations in the integration.
  name: taskConfigs
  type: array
- description: List of trigger configurations.
  name: triggerConfigs
  type: array
- description: Parameters used by the integration.
  name: integrationParameters
  type: array
- description: State of the integration version.
  name: state
  type: string
- description: Output only. Auto-incrementing snapshot number.
  name: snapshotNumber
  type: string
- description: Output only. Time the version was created.
  name: createTime
  type: string
- description: Output only. Email of the last modifier.
  name: lastModifierEmail
  type: string
- description: ID of the template this version was created from.
  name: parentTemplateId
  type: string
- description: User-defined label for the version.
  name: userLabel
  type: string
- description: Database persistence policy for execution logs.
  name: databasePersistencePolicy
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-integration-schema.json
slug: apigee-integration
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Integration Version
---
