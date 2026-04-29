---
description: GetConnectionResponse schema from Amazon Outposts
layout: schema
name: GetConnectionResponse
properties_list:
- description: ''
  name: ConnectionId
  type: object
- description: ''
  name: ConnectionDetails
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-get-connection-response-schema.json
slug: openapi-get-connection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-connection-response-schema.json\",\n  \"title\": \"GetConnectionResponse\",\n  \"description\": \"GetConnectionResponse schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionId\"\n        },\n        {\n          \"description\": \" The ID of the connection. \"\n        }\n      ]\n    },\n    \"ConnectionDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionDetails\"\n        },\n        {\n          \"description\": \" Information about the connection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-connection-response-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: GetConnectionResponse
---
