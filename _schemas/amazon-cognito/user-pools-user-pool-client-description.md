---
description: The description of the user pool client.
layout: schema
name: UserPoolClientDescription
properties_list:
- description: ''
  name: ClientId
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientName
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-pool-client-description-schema.json
slug: user-pools-user-pool-client-description
source_filename: user-pools-user-pool-client-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-client-description-schema.json\",\n  \"title\": \"UserPoolClientDescription\",\n  \"description\": \"The description of the user pool client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The ID of the client associated with the user pool.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to describe the user pool client.\"\n        }\n      ]\n    },\n    \"ClientName\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ClientNameType\"\n        },\n        {\n          \"description\": \"The client name from the user pool client description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-client-description-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UserPoolClientDescription
---
