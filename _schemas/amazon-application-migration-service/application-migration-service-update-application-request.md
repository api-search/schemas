---
description: Request to update a migration application
layout: schema
name: UpdateApplicationRequest
properties_list:
- description: Application ID to update
  name: applicationID
  type: string
- description: New application name
  name: name
  type: string
- description: New application description
  name: description
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-update-application-request-schema.json
slug: application-migration-service-update-application-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-update-application-request-schema.json\",\n  \"title\": \"UpdateApplicationRequest\",\n  \"description\": \"Request to update a migration application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationID\": {\n      \"type\": \"string\",\n      \"description\": \"Application ID to update\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"New application name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"New application description\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-update-application-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: UpdateApplicationRequest
---
