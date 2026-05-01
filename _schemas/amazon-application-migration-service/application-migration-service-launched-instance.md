---
description: Details about the launched EC2 instance
layout: schema
name: LaunchedInstance
properties_list:
- description: EC2 instance ID
  name: ec2InstanceID
  type: string
- description: Job ID that launched this instance
  name: jobID
  type: string
- description: First boot status
  name: firstBoot
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-launched-instance-schema.json
slug: application-migration-service-launched-instance
source_filename: application-migration-service-launched-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-launched-instance-schema.json\",\n  \"title\": \"LaunchedInstance\",\n  \"description\": \"Details about the launched EC2 instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2InstanceID\": {\n      \"type\": \"string\",\n      \"description\": \"EC2 instance ID\"\n    },\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID that launched this instance\"\n    },\n    \"firstBoot\": {\n      \"type\": \"string\",\n      \"description\": \"First boot status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-launched-instance-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: LaunchedInstance
---
