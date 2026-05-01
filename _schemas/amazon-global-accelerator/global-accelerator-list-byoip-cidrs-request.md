---
description: ListByoipCidrsRequest schema from Amazon Global Accelerator API
layout: schema
name: ListByoipCidrsRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-list-byoip-cidrs-request-schema.json
slug: global-accelerator-list-byoip-cidrs-request
source_filename: global-accelerator-list-byoip-cidrs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-byoip-cidrs-request-schema.json\",\n  \"title\": \"ListByoipCidrsRequest\",\n  \"description\": \"ListByoipCidrsRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return with a single call. To retrieve the remaining results, make another call with the returned <code>nextToken</code> value.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The token for the next page of results.\"\n   \
  \     }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-byoip-cidrs-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ListByoipCidrsRequest
---
