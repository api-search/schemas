---
description: Represents the response from the server that lists user pool clients.
layout: schema
name: ListUserPoolClientsResponse
properties_list:
- description: ''
  name: UserPoolClients
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-user-pool-clients-response-schema.json
slug: user-pools-list-user-pool-clients-response
source_filename: user-pools-list-user-pool-clients-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-pool-clients-response-schema.json\",\n  \"title\": \"ListUserPoolClientsResponse\",\n  \"description\": \"Represents the response from the server that lists user pool clients.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolClients\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolClientListType\"\n        },\n        {\n          \"description\": \"The user pool clients in the response that lists user pool clients.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items\
  \ in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-pool-clients-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListUserPoolClientsResponse
---
