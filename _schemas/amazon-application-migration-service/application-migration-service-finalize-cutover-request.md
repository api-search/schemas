---
description: Request to finalize a cutover
layout: schema
name: FinalizeCutoverRequest
properties_list:
- description: Source server ID to finalize cutover for
  name: sourceServerID
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-finalize-cutover-request-schema.json
slug: application-migration-service-finalize-cutover-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-finalize-cutover-request-schema.json\",\n  \"title\": \"FinalizeCutoverRequest\",\n  \"description\": \"Request to finalize a cutover\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID to finalize cutover for\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-finalize-cutover-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: FinalizeCutoverRequest
---
