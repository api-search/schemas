---
description: Summary statistics for blackouts.
layout: schema
name: BlackoutDashboard
properties_list:
- description: Total number of blackouts.
  name: totalBlackouts
  type: integer
- description: Number of currently active blackouts.
  name: activeBlackouts
  type: integer
- description: Number of scheduled future blackouts.
  name: scheduledBlackouts
  type: integer
- description: Number of ended blackouts.
  name: endedBlackouts
  type: integer
- description: Total number of targets currently in blackout.
  name: targetsInBlackout
  type: integer
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-dashboard-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-dashboard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutDashboard\",\n  \"type\": \"object\",\n  \"description\": \"Summary statistics for blackouts.\",\n  \"properties\": {\n    \"totalBlackouts\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of blackouts.\"\n    },\n    \"activeBlackouts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently active blackouts.\"\n    },\n    \"scheduledBlackouts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of scheduled future blackouts.\"\n    },\n    \"endedBlackouts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of ended blackouts.\"\n    },\n    \"targetsInBlackout\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of targets currently in blackout.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-dashboard-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutDashboard
---
