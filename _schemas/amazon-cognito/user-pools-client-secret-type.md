---
description: ClientSecretType schema from Amazon Cognito API
layout: schema
name: ClientSecretType
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-client-secret-type-schema.json
slug: user-pools-client-secret-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-client-secret-type-schema.json\",\n  \"title\": \"ClientSecretType\",\n  \"description\": \"ClientSecretType schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"[\\\\w+]+\",\n  \"minLength\": 1,\n  \"maxLength\": 64\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-client-secret-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ClientSecretType
---
