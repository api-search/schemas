---
description: A migration application grouping source servers
layout: schema
name: Application
properties_list:
- description: Application ID
  name: applicationID
  type: string
- description: ARN of the application
  name: arn
  type: string
- description: Application name
  name: name
  type: string
- description: Application description
  name: description
  type: string
- description: Whether the application is archived
  name: isArchived
  type: boolean
- description: applicationAggregatedStatus
  name: applicationAggregatedStatus
  type: string
- description: Creation date/time
  name: creationDateTime
  type: string
- description: Last modification date/time
  name: lastModifiedDateTime
  type: string
- description: Tags on the application
  name: tags
  type: object
- description: Wave ID this application belongs to
  name: waveID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-application-schema.json
slug: application-migration-service-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"A migration application grouping source servers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationID\": {\n      \"type\": \"string\",\n      \"description\": \"Application ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the application\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Application description\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application is archived\"\n    },\n    \"applicationAggregatedStatus\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"applicationAggregatedStatus\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Creation date/time\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification date/time\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the application\"\n    },\n    \"waveID\": {\n      \"type\": \"string\",\n      \"description\": \"Wave ID this application belongs to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-application-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: Application
---
