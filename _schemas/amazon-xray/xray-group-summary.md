---
description: Details for a group without metadata.
layout: schema
name: GroupSummary
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: GroupARN
  type: object
- description: ''
  name: FilterExpression
  type: object
- description: ''
  name: InsightsConfiguration
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-group-summary-schema.json
slug: xray-group-summary
source_filename: xray-group-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The unique case-sensitive name of the group.\"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the group generated based on the GroupName.\"\n        }\n      ]\n    },\n    \"FilterExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The filter expression defining the parameters to include traces.\"\n        }\n      ]\n    },\n    \"InsightsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightsConfiguration\"\n        },\n        {\n          \"description\": \"<p>The structure\
  \ containing configurations related to insights.</p> <ul> <li> <p>The InsightsEnabled boolean can be set to true to enable insights for the group or false to disable insights for the group.</p> </li> <li> <p>The NotificationsEnabled boolean can be set to true to enable insights notifications. Notifications can only be enabled on a group with InsightsEnabled set to true.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details for a group without metadata.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-group-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-group-summary-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GroupSummary
---
