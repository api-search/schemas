---
description: UpdateResourceServerRequest schema from Amazon Cognito API
layout: schema
name: UpdateResourceServerRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Identifier
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Scopes
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-resource-server-request-schema.json
slug: user-pools-update-resource-server-request
source_filename: user-pools-update-resource-server-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-resource-server-request-schema.json\",\n  \"title\": \"UpdateResourceServerRequest\",\n  \"description\": \"UpdateResourceServerRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerIdentifierType\"\n        },\n        {\n          \"description\": \"The identifier for the resource server.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerNameType\"\
  \n        },\n        {\n          \"description\": \"The name of the resource server.\"\n        }\n      ]\n    },\n    \"Scopes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeListType\"\n        },\n        {\n          \"description\": \"The scope values to be set for the resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Identifier\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-resource-server-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: UpdateResourceServerRequest
---
