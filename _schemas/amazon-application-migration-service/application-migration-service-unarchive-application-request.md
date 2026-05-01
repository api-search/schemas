---
description: Request to unarchive a migration application
layout: schema
name: UnarchiveApplicationRequest
properties_list:
- description: Application ID to unarchive
  name: applicationID
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-unarchive-application-request-schema.json
slug: application-migration-service-unarchive-application-request
source_filename: application-migration-service-unarchive-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-unarchive-application-request-schema.json\",\n  \"title\": \"UnarchiveApplicationRequest\",\n  \"description\": \"Request to unarchive a migration application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationID\": {\n      \"type\": \"string\",\n      \"description\": \"Application ID to unarchive\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-unarchive-application-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: UnarchiveApplicationRequest
---
