---
description: Information about a specified personal access token (PAT).
layout: schema
name: AccessTokenSummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: expiresTime
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-access-token-summary-schema.json
slug: amazon-codecatalyst-access-token-summary
source_filename: amazon-codecatalyst-access-token-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-access-token-summary-schema.json\",\n  \"title\": \"AccessTokenSummary\",\n  \"description\": \"Information about a specified personal access token (PAT).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenId\"\n        },\n        {\n          \"description\": \"The system-generated ID of the personal access token.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenName\"\n        },\n        {\n          \"description\": \"The friendly name of the personal access token.\"\n        }\n      ]\n    },\n    \"expiresTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\
  \n        },\n        {\n          \"description\": \"The date and time when the personal access token will expire, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-access-token-summary-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: AccessTokenSummary
---
