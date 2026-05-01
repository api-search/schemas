---
description: A log entry for a migration job
layout: schema
name: JobLogItem
properties_list:
- description: Date/time of the log entry
  name: logDateTime
  type: string
- description: Log event type
  name: event
  type: string
- description: eventData
  name: eventData
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-job-log-item-schema.json
slug: application-migration-service-job-log-item
source_filename: application-migration-service-job-log-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-job-log-item-schema.json\",\n  \"title\": \"JobLogItem\",\n  \"description\": \"A log entry for a migration job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of the log entry\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Log event type\"\n    },\n    \"eventData\": {\n      \"type\": \"string\",\n      \"description\": \"eventData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-job-log-item-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: JobLogItem
---
