---
description: Replication initiation steps and their status
layout: schema
name: DataReplicationInitiation
properties_list:
- description: Date/time replication initiation started
  name: startDateTime
  type: string
- description: Date/time of next retry attempt
  name: nextAttemptDateTime
  type: string
- description: Initiation steps
  name: steps
  type: array
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-data-replication-initiation-schema.json
slug: application-migration-service-data-replication-initiation
source_filename: application-migration-service-data-replication-initiation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-data-replication-initiation-schema.json\",\n  \"title\": \"DataReplicationInitiation\",\n  \"description\": \"Replication initiation steps and their status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time replication initiation started\"\n    },\n    \"nextAttemptDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of next retry attempt\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Initiation steps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-data-replication-initiation-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DataReplicationInitiation
---
