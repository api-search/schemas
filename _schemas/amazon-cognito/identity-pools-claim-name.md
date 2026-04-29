---
description: ClaimName schema from Amazon Cognito API
layout: schema
name: ClaimName
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-claim-name-schema.json
slug: identity-pools-claim-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-claim-name-schema.json\",\n  \"title\": \"ClaimName\",\n  \"description\": \"ClaimName schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n  \"minLength\": 1,\n  \"maxLength\": 64\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-claim-name-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ClaimName
---
