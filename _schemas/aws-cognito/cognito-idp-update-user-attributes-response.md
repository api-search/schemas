---
description: Represents the response from the server for the request to update user attributes.
layout: schema
name: UpdateUserAttributesResponse
properties_list:
- description: ''
  name: CodeDeliveryDetailsList
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-update-user-attributes-response-schema.json
slug: cognito-idp-update-user-attributes-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetailsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsListType\"\n        },\n        {\n          \"description\": \"The code delivery details list from the server for the request to update user attributes.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response from the server for the request to update user attributes.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-user-attributes-response-schema.json\",\n  \"title\": \"UpdateUserAttributesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-user-attributes-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UpdateUserAttributesResponse
---
