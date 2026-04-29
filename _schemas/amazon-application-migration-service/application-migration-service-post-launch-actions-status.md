---
description: Status of post-launch actions
layout: schema
name: PostLaunchActionsStatus
properties_list:
- description: List of post-launch action statuses
  name: postLaunchActionsLaunchStatusList
  type: array
- description: Date/time SSM agent was discovered
  name: ssmAgentDiscoveryDatetime
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-post-launch-actions-status-schema.json
slug: application-migration-service-post-launch-actions-status
source_filename: application-migration-service-post-launch-actions-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-post-launch-actions-status-schema.json\",\n  \"title\": \"PostLaunchActionsStatus\",\n  \"description\": \"Status of post-launch actions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"postLaunchActionsLaunchStatusList\": {\n      \"type\": \"array\",\n      \"description\": \"List of post-launch action statuses\"\n    },\n    \"ssmAgentDiscoveryDatetime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time SSM agent was discovered\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-post-launch-actions-status-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: PostLaunchActionsStatus
---
