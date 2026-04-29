---
description: Request to terminate test or cutover instances
layout: schema
name: TerminateTargetInstancesRequest
properties_list:
- description: Source server IDs whose instances to terminate
  name: sourceServerIDs
  type: array
- description: Tags for the termination job
  name: tags
  type: object
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-terminate-target-instances-request-schema.json
slug: application-migration-service-terminate-target-instances-request
source_filename: application-migration-service-terminate-target-instances-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-terminate-target-instances-request-schema.json\",\n  \"title\": \"TerminateTargetInstancesRequest\",\n  \"description\": \"Request to terminate test or cutover instances\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Source server IDs whose instances to terminate\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for the termination job\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-terminate-target-instances-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: TerminateTargetInstancesRequest
---
