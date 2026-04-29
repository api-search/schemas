---
description: Request body for creating a new blackout.
layout: schema
name: BlackoutCreateRequest
properties_list:
- description: Display name for the blackout.
  name: blackoutName
  type: string
- description: Description of the blackout purpose.
  name: description
  type: string
- description: Reason for the blackout.
  name: reason
  type: string
- description: List of targets to include in the blackout.
  name: targets
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-create-request-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-create-request
source_filename: oracle-enterprise-manager-cloud-control-blackout-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new blackout.\",\n  \"properties\": {\n    \"blackoutName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the blackout.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the blackout purpose.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the blackout.\"\n    },\n    \"targets\": {\n      \"type\": \"array\",\n      \"description\": \"List of targets to include in the blackout.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-create-request-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutCreateRequest
---
