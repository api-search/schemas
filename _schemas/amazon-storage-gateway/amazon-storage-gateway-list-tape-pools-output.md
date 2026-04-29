---
description: ListTapePoolsOutput schema from Amazon Storage Gateway API
layout: schema
name: ListTapePoolsOutput
properties_list:
- description: ''
  name: PoolInfos
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-tape-pools-output-schema.json
slug: amazon-storage-gateway-list-tape-pools-output
source_filename: amazon-storage-gateway-list-tape-pools-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tape-pools-output-schema.json\",\n  \"title\": \"ListTapePoolsOutput\",\n  \"description\": \"ListTapePoolsOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolInfos\"\n        },\n        {\n          \"description\": \"An array of <code>PoolInfo</code> objects, where each object describes a single custom tape pool. If there are no custom tape pools, the <code>PoolInfos</code> is an empty array. \"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A string that indicates the position at which to\
  \ begin the returned list of tape pools. Use the marker in your next request to continue pagination of tape pools. If there are no more tape pools to list, this element does not appear in the response body. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tape-pools-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListTapePoolsOutput
---
