---
description: ListSyncResourcesRequest schema
layout: schema
name: ListSyncResourcesRequest
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-sync-resources-request-schema.json
slug: iot-twinmaker-list-sync-resources-request
source_filename: iot-twinmaker-list-sync-resources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-resources-request-schema.json\",\n  \"title\": \"ListSyncResourcesRequest\",\n  \"description\": \"ListSyncResourcesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceFilters\"\n        },\n        {\n          \"description\": \"<p>A list of objects that filter the request.</p> <p>The following filter combinations are supported:</p> <ul> <li> <p>Filter with state</p> </li> <li> <p>Filter with ResourceType and ResourceId</p> </li> <li> <p>Filter with ResourceType and ExternalId</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n\
  \          \"description\": \"<p>The maximum number of results to return at one time. The default is 50.</p> <p>Valid Range: Minimum value of 0. Maximum value of 200.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-resources-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListSyncResourcesRequest
---
