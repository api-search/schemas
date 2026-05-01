---
description: ArnType schema from Amazon Cognito API
layout: schema
name: ArnType
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-arn-type-schema.json
slug: user-pools-arn-type
source_filename: user-pools-arn-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-arn-type-schema.json\",\n  \"title\": \"ArnType\",\n  \"description\": \"ArnType schema from Amazon Cognito API\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:[\\\\w+=/,.@-]+:[\\\\w+=/,.@-]+:([\\\\w+=/,.@-]*)?:[0-9]+:[\\\\w+=/,.@-]+(:[\\\\w+=/,.@-]+)?(:[\\\\w+=/,.@-]+)?\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-arn-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ArnType
---
