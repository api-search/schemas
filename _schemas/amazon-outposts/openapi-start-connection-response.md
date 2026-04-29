---
description: StartConnectionResponse schema from Amazon Outposts
layout: schema
name: StartConnectionResponse
properties_list:
- description: ''
  name: ConnectionId
  type: object
- description: ''
  name: UnderlayIpAddress
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-start-connection-response-schema.json
slug: openapi-start-connection-response
source_filename: openapi-start-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-start-connection-response-schema.json\",\n  \"title\": \"StartConnectionResponse\",\n  \"description\": \"StartConnectionResponse schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionId\"\n        },\n        {\n          \"description\": \" The ID of the connection. \"\n        }\n      ]\n    },\n    \"UnderlayIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnderlayIpAddress\"\n        },\n        {\n          \"description\": \" The underlay IP address. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-start-connection-response-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: StartConnectionResponse
---
