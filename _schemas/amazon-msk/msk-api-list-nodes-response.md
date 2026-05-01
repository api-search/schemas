---
description: ListNodesResponse schema from Amazon MSK API
layout: schema
name: ListNodesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: NodeInfoList
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-nodes-response-schema.json
slug: msk-api-list-nodes-response
source_filename: msk-api-list-nodes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-nodes-response-schema.json\",\n  \"title\": \"ListNodesResponse\",\n  \"description\": \"ListNodesResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"\\n            <p>The paginated results marker. When the result of a ListNodes operation is truncated, the call returns NextToken in the response. \\n               To get another batch of nodes, provide this token in your next request.</p>\"\n        }\n      ]\n    },\n    \"NodeInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfNodeInfo\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"nodeInfoList\"\n          },\n          \"description\": \"\\n            <p>List containing a NodeInfo object.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-nodes-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListNodesResponse
---
