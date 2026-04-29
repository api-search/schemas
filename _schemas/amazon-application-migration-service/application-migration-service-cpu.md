---
description: CPU information for a source server
layout: schema
name: CPU
properties_list:
- description: Number of cores
  name: cores
  type: integer
- description: CPU model name
  name: modelName
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-cpu-schema.json
slug: application-migration-service-cpu
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-cpu-schema.json\",\n  \"title\": \"CPU\",\n  \"description\": \"CPU information for a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cores\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cores\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"CPU model name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-cpu-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: CPU
---
