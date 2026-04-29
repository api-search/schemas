---
description: A RHEL system registered with Red Hat Insights for monitoring and recommendations.
layout: schema
name: System
properties_list:
- description: The unique identifier of the system.
  name: system_uuid
  type: string
- description: The display name of the system.
  name: display_name
  type: string
- description: The last time the system checked in with Insights.
  name: last_seen
  type: string
- description: The date when the system will be considered stale.
  name: stale_at
  type: string
- description: The number of active Advisor recommendations.
  name: hits
  type: integer
- description: The number of critical severity recommendations.
  name: critical_hits
  type: integer
- description: The number of important severity recommendations.
  name: important_hits
  type: integer
- description: The number of moderate severity recommendations.
  name: moderate_hits
  type: integer
- description: The number of low severity recommendations.
  name: low_hits
  type: integer
- description: The RHEL version running on the system.
  name: rhel_version
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-system-schema.json
slug: red-hat-insights-system
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"System\",\n  \"type\": \"object\",\n  \"description\": \"A RHEL system registered with Red Hat Insights for monitoring and recommendations.\",\n  \"properties\": {\n    \"system_uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the system.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the system.\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"description\": \"The last time the system checked in with Insights.\"\n    },\n    \"stale_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date when the system will be considered stale.\"\n    },\n    \"hits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of active Advisor recommendations.\"\n    },\n    \"critical_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number\
  \ of critical severity recommendations.\"\n    },\n    \"important_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of important severity recommendations.\"\n    },\n    \"moderate_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of moderate severity recommendations.\"\n    },\n    \"low_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of low severity recommendations.\"\n    },\n    \"rhel_version\": {\n      \"type\": \"string\",\n      \"description\": \"The RHEL version running on the system.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-system-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: System
---
