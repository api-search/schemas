---
description: Provides information about the context in which temporary security credentials were issued to an entity.
layout: schema
name: SessionContextAttributes
properties_list:
- description: ''
  name: creationDate
  type: object
- description: ''
  name: mfaAuthenticated
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-session-context-attributes-schema.json
slug: amazon-macie-session-context-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-context-attributes-schema.json\",\n  \"title\": \"SessionContextAttributes\",\n  \"description\": \"Provides information about the context in which temporary security credentials were issued to an entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and ISO 8601 format, when the credentials were issued.\"\n        }\n      ]\n    },\n    \"mfaAuthenticated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the credentials were authenticated with a multi-factor authentication\
  \ (MFA) device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-context-attributes-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SessionContextAttributes
---
