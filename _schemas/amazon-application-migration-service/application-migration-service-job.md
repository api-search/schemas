---
description: A migration or conversion job
layout: schema
name: Job
properties_list:
- description: Job ID
  name: jobID
  type: string
- description: ARN of the job
  name: arn
  type: string
- description: Job type
  name: type
  type: string
- description: Who initiated the job
  name: initiatedBy
  type: string
- description: Date/time job was created
  name: creationDateTime
  type: string
- description: Date/time job ended
  name: endDateTime
  type: string
- description: Job status
  name: status
  type: string
- description: Servers participating in the job
  name: participatingServers
  type: array
- description: Tags on the job
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-job-schema.json
slug: application-migration-service-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"A migration or conversion job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the job\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Job type\"\n    },\n    \"initiatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Who initiated the job\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time job was created\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time job ended\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Job status\"\n    },\n    \"participatingServers\": {\n      \"type\": \"array\",\n      \"description\": \"Servers participating in the job\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the job\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-job-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: Job
---
