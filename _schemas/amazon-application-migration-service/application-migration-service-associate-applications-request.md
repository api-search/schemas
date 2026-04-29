---
description: Request to associate applications with a wave
layout: schema
name: AssociateApplicationsRequest
properties_list:
- description: Wave ID
  name: waveID
  type: string
- description: Application IDs to associate
  name: applicationIDs
  type: array
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-associate-applications-request-schema.json
slug: application-migration-service-associate-applications-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-associate-applications-request-schema.json\",\n  \"title\": \"AssociateApplicationsRequest\",\n  \"description\": \"Request to associate applications with a wave\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waveID\": {\n      \"type\": \"string\",\n      \"description\": \"Wave ID\"\n    },\n    \"applicationIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Application IDs to associate\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-associate-applications-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: AssociateApplicationsRequest
---
