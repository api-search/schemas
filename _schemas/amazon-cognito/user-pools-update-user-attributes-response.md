---
description: Represents the response from the server for the request to update user attributes.
layout: schema
name: UpdateUserAttributesResponse
properties_list:
- description: ''
  name: CodeDeliveryDetailsList
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-user-attributes-response-schema.json
slug: user-pools-update-user-attributes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-attributes-response-schema.json\",\n  \"title\": \"UpdateUserAttributesResponse\",\n  \"description\": \"Represents the response from the server for the request to update user attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetailsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsListType\"\n        },\n        {\n          \"description\": \"The code delivery details list from the server for the request to update user attributes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-attributes-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateUserAttributesResponse
---
