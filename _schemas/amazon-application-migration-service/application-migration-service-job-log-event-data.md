---
description: Data associated with a job log event
layout: schema
name: JobLogEventData
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Conversion server ID
  name: conversionServerID
  type: string
- description: Target EC2 instance ID
  name: targetInstanceID
  type: string
- description: Raw error message if applicable
  name: rawError
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-job-log-event-data-schema.json
slug: application-migration-service-job-log-event-data
source_filename: application-migration-service-job-log-event-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-job-log-event-data-schema.json\",\n  \"title\": \"JobLogEventData\",\n  \"description\": \"Data associated with a job log event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"conversionServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Conversion server ID\"\n    },\n    \"targetInstanceID\": {\n      \"type\": \"string\",\n      \"description\": \"Target EC2 instance ID\"\n    },\n    \"rawError\": {\n      \"type\": \"string\",\n      \"description\": \"Raw error message if applicable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-job-log-event-data-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: JobLogEventData
---
