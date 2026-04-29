---
description: Provides information about a session that was created for an entity that performed an action by using temporary security credentials.
layout: schema
name: SessionContext
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: sessionIssuer
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-session-context-schema.json
slug: amazon-macie-session-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-context-schema.json\",\n  \"title\": \"SessionContext\",\n  \"description\": \"Provides information about a session that was created for an entity that performed an action by using temporary security credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionContextAttributes\"\n        },\n        {\n          \"description\": \"The date and time when the credentials were issued, and whether the credentials were authenticated with a multi-factor authentication (MFA) device.\"\n        }\n      ]\n    },\n    \"sessionIssuer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionIssuer\"\n        },\n        {\n          \"description\": \"The source\
  \ and type of credentials that were issued to the entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-context-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SessionContext
---
