---
description: An optimization activity for creative optimization.
layout: schema
name: OptimizationActivity
properties_list:
- description: Floodlight activity ID of this optimization activity.
  name: floodlightActivityId
  type: string
- description: Weight associated with this optimization.
  name: weight
  type: integer
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-optimization-activity-schema.json
slug: google-campaign-manager-optimization-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OptimizationActivity\",\n  \"type\": \"object\",\n  \"description\": \"An optimization activity for creative optimization.\",\n  \"properties\": {\n    \"floodlightActivityId\": {\n      \"type\": \"string\",\n      \"description\": \"Floodlight activity ID of this optimization activity.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight associated with this optimization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-optimization-activity-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: OptimizationActivity
---
