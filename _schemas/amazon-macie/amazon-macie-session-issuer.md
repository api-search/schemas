---
description: Provides information about the source and type of temporary security credentials that were issued to an entity.
layout: schema
name: SessionIssuer
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: principalId
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: userName
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-session-issuer-schema.json
slug: amazon-macie-session-issuer
source_filename: amazon-macie-session-issuer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-issuer-schema.json\",\n  \"title\": \"SessionIssuer\",\n  \"description\": \"Provides information about the source and type of temporary security credentials that were issued to an entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that owns the entity that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the source account, Identity and Access Management (IAM) user,\
  \ or role that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"principalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the entity that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The source of the temporary security credentials, such as Root, IAMUser, or Role.\"\n        }\n      ]\n    },\n    \"userName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name or alias of the user or role that issued the session. This value is null if the credentials were obtained from a root account that doesn't have an alias.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-session-issuer-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SessionIssuer
---
