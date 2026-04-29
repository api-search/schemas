---
description: Request to mark a source server as archived
layout: schema
name: MarkAsArchivedRequest
properties_list:
- description: Source server ID to archive
  name: sourceServerID
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-mark-as-archived-request-schema.json
slug: application-migration-service-mark-as-archived-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-mark-as-archived-request-schema.json\",\n  \"title\": \"MarkAsArchivedRequest\",\n  \"description\": \"Request to mark a source server as archived\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID to archive\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-mark-as-archived-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: MarkAsArchivedRequest
---
