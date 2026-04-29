---
description: IdentityId schema from Amazon Cognito API
layout: schema
name: IdentityId
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-identity-id-schema.json
slug: identity-pools-identity-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-id-schema.json\",\n  \"title\": \"IdentityId\",\n  \"description\": \"IdentityId schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\w-]+:[0-9a-f-]+\",\n  \"minLength\": 1,\n  \"maxLength\": 55\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-id-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: IdentityId
---
