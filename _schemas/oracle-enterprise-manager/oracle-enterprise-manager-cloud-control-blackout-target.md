---
description: A target included in a blackout.
layout: schema
name: BlackoutTarget
properties_list:
- description: Name of the target.
  name: targetName
  type: string
- description: Type of the target.
  name: targetType
  type: string
- description: Whether to include member targets (for composite targets and groups).
  name: includeMembers
  type: boolean
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-target-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutTarget\",\n  \"type\": \"object\",\n  \"description\": \"A target included in a blackout.\",\n  \"properties\": {\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the target.\"\n    },\n    \"includeMembers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include member targets (for composite targets and groups).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-target-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutTarget
---
