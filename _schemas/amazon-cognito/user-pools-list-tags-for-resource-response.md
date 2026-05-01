---
description: ListTagsForResourceResponse schema from Amazon Cognito API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-tags-for-resource-response-schema.json
slug: user-pools-list-tags-for-resource-response
source_filename: user-pools-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolTagsType\"\n        },\n        {\n          \"description\": \"The tags that are assigned to the user pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-tags-for-resource-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ListTagsForResourceResponse
---
