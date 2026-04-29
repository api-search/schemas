---
description: A migration wave grouping applications
layout: schema
name: Wave
properties_list:
- description: Wave ID
  name: waveID
  type: string
- description: ARN of the wave
  name: arn
  type: string
- description: Wave name
  name: name
  type: string
- description: Wave description
  name: description
  type: string
- description: Whether the wave is archived
  name: isArchived
  type: boolean
- description: waveAggregatedStatus
  name: waveAggregatedStatus
  type: string
- description: Creation date/time
  name: creationDateTime
  type: string
- description: Last modification date/time
  name: lastModifiedDateTime
  type: string
- description: Tags on the wave
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-wave-schema.json
slug: application-migration-service-wave
source_filename: application-migration-service-wave-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-wave-schema.json\",\n  \"title\": \"Wave\",\n  \"description\": \"A migration wave grouping applications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waveID\": {\n      \"type\": \"string\",\n      \"description\": \"Wave ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the wave\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Wave name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Wave description\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the wave is archived\"\n    },\n    \"waveAggregatedStatus\": {\n      \"type\": \"string\",\n      \"description\": \"waveAggregatedStatus\"\n    },\n    \"creationDateTime\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Creation date/time\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification date/time\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the wave\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-wave-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: Wave
---
