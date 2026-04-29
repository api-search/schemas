---
description: QueryArn schema
layout: schema
name: QueryArn
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-query-arn-schema.json
slug: config-query-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-query-arn-schema.json\",\n  \"title\": \"QueryArn\",\n  \"description\": \"QueryArn schema\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[a-z\\\\-]*:config:[a-z\\\\-\\\\d]+:\\\\d+:stored-query/[a-zA-Z0-9-_]+/query-[a-zA-Z\\\\d-_/]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 500\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-query-arn-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: QueryArn
---
