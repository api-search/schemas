---
description: Provides information about an identity that performed an action on an affected resource by using temporary security credentials. The credentials were obtained using the AssumeRole operation of the Security Token Service (STS) API.
layout: schema
name: AssumedRole
properties_list:
- description: ''
  name: accessKeyId
  type: object
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
  name: sessionContext
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-assumed-role-schema.json
slug: amazon-macie-assumed-role
source_filename: amazon-macie-assumed-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-assumed-role-schema.json\",\n  \"title\": \"AssumedRole\",\n  \"description\": \"Provides information about an identity that performed an action on an affected resource by using temporary security credentials. The credentials were obtained using the AssumeRole operation of the Security Token Service (STS) API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services access key ID that identifies the credentials.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier\
  \ for the Amazon Web Services account that owns the entity that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the entity that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"principalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the entity that was used to get the credentials.\"\n        }\n      ]\n    },\n    \"sessionContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionContext\"\n        },\n        {\n          \"description\": \"The details of the session that was created for the credentials, including the entity that issued the session.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-assumed-role-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AssumedRole
---
