---
description: <p>A JSON object that contains one or more of the following fields:</p> <ul> <li> <p> <a>ListTapesInput$Limit</a> </p> </li> <li> <p> <a>ListTapesInput$Marker</a> </p> </li> <li> <p> <a>ListTapesInput$TapeARNs</a> </p> </li> </ul>
layout: schema
name: ListTapesInput
properties_list:
- description: ''
  name: TapeARNs
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-tapes-input-schema.json
slug: amazon-storage-gateway-list-tapes-input
source_filename: amazon-storage-gateway-list-tapes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tapes-input-schema.json\",\n  \"title\": \"ListTapesInput\",\n  \"description\": \"<p>A JSON object that contains one or more of the following fields:</p> <ul> <li> <p> <a>ListTapesInput$Limit</a> </p> </li> <li> <p> <a>ListTapesInput$Marker</a> </p> </li> <li> <p> <a>ListTapesInput$TapeARNs</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARNs\": {\n      \"$ref\": \"#/components/schemas/TapeARNs\"\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A string that indicates the position at which to begin the returned list of tapes.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"An optional number limit for the tapes in the list returned by this call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tapes-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListTapesInput
---
