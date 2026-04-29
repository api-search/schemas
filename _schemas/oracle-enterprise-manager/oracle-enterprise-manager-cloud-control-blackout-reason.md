---
description: A predefined reason for blackouts.
layout: schema
name: BlackoutReason
properties_list:
- description: Unique identifier for the reason.
  name: reasonId
  type: string
- description: Text of the blackout reason.
  name: reason
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-reason-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-reason
source_filename: oracle-enterprise-manager-cloud-control-blackout-reason-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutReason\",\n  \"type\": \"object\",\n  \"description\": \"A predefined reason for blackouts.\",\n  \"properties\": {\n    \"reasonId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the reason.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Text of the blackout reason.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-reason-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutReason
---
