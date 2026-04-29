---
description: ListResourceServersResponse schema from Amazon Cognito API
layout: schema
name: ListResourceServersResponse
properties_list:
- description: ''
  name: ResourceServers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-resource-servers-response-schema.json
slug: user-pools-list-resource-servers-response
source_filename: user-pools-list-resource-servers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-resource-servers-response-schema.json\",\n  \"title\": \"ListResourceServersResponse\",\n  \"description\": \"ListResourceServersResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServersListType\"\n        },\n        {\n          \"description\": \"The resource servers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-resource-servers-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListResourceServersResponse
---
