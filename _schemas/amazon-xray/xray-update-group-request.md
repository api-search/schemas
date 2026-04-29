---
description: UpdateGroupRequest schema from Amazon X-Ray API
layout: schema
name: UpdateGroupRequest
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
schema_file: json-schema/xray-update-group-request-schema.json
slug: xray-update-group-request
source_filename: xray-update-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateGroupRequest\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The case-sensitive name of the group.\"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupARN\"\n        },\n        {\n          \"description\": \"The ARN that was generated upon creation.\"\n        }\n      ]\n    },\n    \"FilterExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterExpression\"\n        },\n        {\n          \"description\": \"The updated filter expression defining criteria by which to group traces.\"\n        }\n      ]\n    },\n    \"InsightsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightsConfiguration\"\n        },\n        {\n  \
  \        \"description\": \"<p>The structure containing configurations related to insights.</p> <ul> <li> <p>The InsightsEnabled boolean can be set to true to enable insights for the group or false to disable insights for the group.</p> </li> <li> <p>The NotificationsEnabled boolean can be set to true to enable insights notifications for the group. Notifications can only be enabled on a group with InsightsEnabled set to true.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-group-request-schema.json\",\n  \"description\": \"UpdateGroupRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-group-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UpdateGroupRequest
---
