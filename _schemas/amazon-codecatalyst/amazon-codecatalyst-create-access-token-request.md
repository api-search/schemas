---
description: CreateAccessTokenRequest schema from Amazon CodeCatalyst
layout: schema
name: CreateAccessTokenRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: expiresTime
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-access-token-request-schema.json
slug: amazon-codecatalyst-create-access-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-access-token-request-schema.json\",\n  \"title\": \"CreateAccessTokenRequest\",\n  \"description\": \"CreateAccessTokenRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenName\"\n        },\n        {\n          \"description\": \"The friendly name of the personal access token.\"\n        }\n      ]\n    },\n    \"expiresTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The date and time the personal access token expires, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\
  \">RFC 3339</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-access-token-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateAccessTokenRequest
---
