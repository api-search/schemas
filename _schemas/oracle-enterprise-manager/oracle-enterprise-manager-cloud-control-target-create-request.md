---
description: Request body for creating a new target.
layout: schema
name: TargetCreateRequest
properties_list:
- description: Display name for the target.
  name: targetName
  type: string
- description: Target type identifier defining the monitoring template.
  name: targetType
  type: string
- description: The hostname where the target resides.
  name: hostName
  type: string
- description: Target-type-specific properties required for monitoring.
  name: properties
  type: object
- description: Monitoring credentials for the target.
  name: credentials
  type: object
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-target-create-request-schema.json
slug: oracle-enterprise-manager-cloud-control-target-create-request
source_filename: oracle-enterprise-manager-cloud-control-target-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new target.\",\n  \"properties\": {\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the target.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Target type identifier defining the monitoring template.\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname where the target resides.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Target-type-specific properties required for monitoring.\"\n    },\n    \"credentials\": {\n      \"type\": \"object\",\n      \"description\": \"Monitoring credentials for the target.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-target-create-request-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: TargetCreateRequest
---
