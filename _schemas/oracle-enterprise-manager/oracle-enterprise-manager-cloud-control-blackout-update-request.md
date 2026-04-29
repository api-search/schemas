---
description: Request body for updating a blackout.
layout: schema
name: BlackoutUpdateRequest
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: targets
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-update-request-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a blackout.\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"targets\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-update-request-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutUpdateRequest
---
