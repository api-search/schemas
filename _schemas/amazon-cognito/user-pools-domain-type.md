---
description: DomainType schema from Amazon Cognito API
layout: schema
name: DomainType
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-domain-type-schema.json
slug: user-pools-domain-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-domain-type-schema.json\",\n  \"title\": \"DomainType\",\n  \"description\": \"DomainType schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"pattern\": \"^[a-z0-9](?:[a-z0-9\\\\-]{0,61}[a-z0-9])?$\",\n  \"minLength\": 1,\n  \"maxLength\": 63\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-domain-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DomainType
---
