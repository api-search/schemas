---
description: Licensing settings for the launched instance
layout: schema
name: Licensing
properties_list:
- description: Whether to use Bring Your Own License for the OS
  name: osByol
  type: boolean
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-licensing-schema.json
slug: application-migration-service-licensing
source_filename: application-migration-service-licensing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-licensing-schema.json\",\n  \"title\": \"Licensing\",\n  \"description\": \"Licensing settings for the launched instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"osByol\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use Bring Your Own License for the OS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-licensing-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: Licensing
---
