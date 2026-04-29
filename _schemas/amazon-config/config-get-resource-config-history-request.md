---
description: The input for the <a>GetResourceConfigHistory</a> action.
layout: schema
name: GetResourceConfigHistoryRequest
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: laterTime
  type: object
- description: ''
  name: earlierTime
  type: object
- description: ''
  name: chronologicalOrder
  type: object
- description: ''
  name: limit
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-resource-config-history-request-schema.json
slug: config-get-resource-config-history-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-config-history-request-schema.json\",\n  \"title\": \"GetResourceConfigHistoryRequest\",\n  \"description\": \"The input for the <a>GetResourceConfigHistory</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The resource type.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the resource (for example., <code>sg-xxxxxx</code>).\"\n        }\n      ]\n    },\n    \"laterTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaterTime\"\
  \n        },\n        {\n          \"description\": \"The time stamp that indicates a later time. If not specified, current time is taken.\"\n        }\n      ]\n    },\n    \"earlierTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EarlierTime\"\n        },\n        {\n          \"description\": \"The time stamp that indicates an earlier time. If not specified, the action returns paginated results that contain configuration items that start when the first configuration item was recorded.\"\n        }\n      ]\n    },\n    \"chronologicalOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChronologicalOrder\"\n        },\n        {\n          \"description\": \"The chronological order for configuration items listed. By default, the results are listed in reverse chronological order.\"\n        }\n      ]\n    },\n    \"limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n     \
  \   },\n        {\n          \"description\": \"The maximum number of configuration items returned on each page. The default is 10. You cannot specify a number greater than 100. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\",\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-config-history-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetResourceConfigHistoryRequest
---
