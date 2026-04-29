---
description: UsernameType schema from Amazon Cognito API
layout: schema
name: UsernameType
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-username-type-schema.json
slug: user-pools-username-type
source_filename: user-pools-username-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-username-type-schema.json\",\n  \"title\": \"UsernameType\",\n  \"description\": \"UsernameType schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n  \"minLength\": 1,\n  \"maxLength\": 128\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-username-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UsernameType
---
