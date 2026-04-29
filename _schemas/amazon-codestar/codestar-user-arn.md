---
description: UserArn schema from AWS CodeStar API
layout: schema
name: UserArn
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-user-arn-schema.json
slug: codestar-user-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-user-arn-schema.json\",\n  \"title\": \"UserArn\",\n  \"description\": \"UserArn schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws:iam::\\\\d{12}:user(?:(\\\\u002F)|(\\\\u002F[\\\\u0021-\\\\u007E]+\\\\u002F))[\\\\w+=,.@-]+$\",\n  \"minLength\": 32,\n  \"maxLength\": 95\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-user-arn-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: UserArn
---
