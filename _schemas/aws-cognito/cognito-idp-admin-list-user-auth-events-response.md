---
description: AdminListUserAuthEventsResponse schema from Amazon Cognito
layout: schema
name: AdminListUserAuthEventsResponse
properties_list:
- description: ''
  name: AuthEvents
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-list-user-auth-events-response-schema.json
slug: cognito-idp-admin-list-user-auth-events-response
source_filename: cognito-idp-admin-list-user-auth-events-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthEventsType\"\n        },\n        {\n          \"description\": \"The response object. It includes the <code>EventID</code>, <code>EventType</code>, <code>CreationDate</code>, <code>EventRisk</code>, and <code>EventResponse</code>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-list-user-auth-events-response-schema.json\",\n  \"title\": \"AdminListUserAuthEventsResponse\",\n  \"description\": \"AdminListUserAuthEventsResponse schema from Amazon\
  \ Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-list-user-auth-events-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminListUserAuthEventsResponse
---
