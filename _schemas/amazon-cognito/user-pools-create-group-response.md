---
description: CreateGroupResponse schema from Amazon Cognito API
layout: schema
name: CreateGroupResponse
properties_list:
- description: ''
  name: Group
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-group-response-schema.json
slug: user-pools-create-group-response
source_filename: user-pools-create-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-group-response-schema.json\",\n  \"title\": \"CreateGroupResponse\",\n  \"description\": \"CreateGroupResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupType\"\n        },\n        {\n          \"description\": \"The group object for the group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-group-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CreateGroupResponse
---
