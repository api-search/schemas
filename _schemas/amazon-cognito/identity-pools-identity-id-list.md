---
description: IdentityIdList schema from Amazon Cognito API
layout: schema
name: IdentityIdList
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-identity-id-list-schema.json
slug: identity-pools-identity-id-list
source_filename: identity-pools-identity-id-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-id-list-schema.json\",\n  \"title\": \"IdentityIdList\",\n  \"description\": \"IdentityIdList schema from Amazon Cognito API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/IdentityId\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 60\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-id-list-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: IdentityIdList
---
