---
description: A server participating in a migration job
layout: schema
name: ParticipatingServer
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Launch status
  name: launchStatus
  type: string
- description: Launched EC2 instance ID
  name: launchedEc2InstanceID
  type: string
- description: postLaunchActionsStatus
  name: postLaunchActionsStatus
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-participating-server-schema.json
slug: application-migration-service-participating-server
source_filename: application-migration-service-participating-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-participating-server-schema.json\",\n  \"title\": \"ParticipatingServer\",\n  \"description\": \"A server participating in a migration job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"launchStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Launch status\"\n    },\n    \"launchedEc2InstanceID\": {\n      \"type\": \"string\",\n      \"description\": \"Launched EC2 instance ID\"\n    },\n    \"postLaunchActionsStatus\": {\n      \"type\": \"string\",\n      \"description\": \"postLaunchActionsStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-participating-server-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ParticipatingServer
---
