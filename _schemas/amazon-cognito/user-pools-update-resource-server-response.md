---
description: UpdateResourceServerResponse schema from Amazon Cognito API
layout: schema
name: UpdateResourceServerResponse
properties_list:
- description: ''
  name: ResourceServer
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-resource-server-response-schema.json
slug: user-pools-update-resource-server-response
source_filename: user-pools-update-resource-server-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-resource-server-response-schema.json\",\n  \"title\": \"UpdateResourceServerResponse\",\n  \"description\": \"UpdateResourceServerResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerType\"\n        },\n        {\n          \"description\": \"The resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServer\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-resource-server-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateResourceServerResponse
---
