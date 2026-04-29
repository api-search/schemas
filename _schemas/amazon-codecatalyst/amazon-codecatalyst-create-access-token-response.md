---
description: CreateAccessTokenResponse schema from Amazon CodeCatalyst
layout: schema
name: CreateAccessTokenResponse
properties_list:
- description: ''
  name: secret
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: expiresTime
  type: object
- description: ''
  name: accessTokenId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-access-token-response-schema.json
slug: amazon-codecatalyst-create-access-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-access-token-response-schema.json\",\n  \"title\": \"CreateAccessTokenResponse\",\n  \"description\": \"CreateAccessTokenResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"secret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenSecret\"\n        },\n        {\n          \"description\": \"The secret value of the personal access token.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenName\"\n        },\n        {\n          \"description\": \"The friendly name of the personal access token.\"\n        }\n      ]\n    },\n    \"expiresTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\
  \n        },\n        {\n          \"description\": \"The date and time the personal access token expires, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>. If not specified, the default is one year from creation.\"\n        }\n      ]\n    },\n    \"accessTokenId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenId\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the access token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"secret\",\n    \"name\",\n    \"expiresTime\",\n    \"accessTokenId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-access-token-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateAccessTokenResponse
---
