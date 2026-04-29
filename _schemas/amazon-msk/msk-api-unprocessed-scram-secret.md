---
description: <p>Error info for scram secret associate/disassociate failure.</p>
layout: schema
name: UnprocessedScramSecret
properties_list:
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: SecretArn
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-unprocessed-scram-secret-schema.json
slug: msk-api-unprocessed-scram-secret
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-unprocessed-scram-secret-schema.json\",\n  \"title\": \"UnprocessedScramSecret\",\n  \"description\": \"\\n            <p>Error info for scram secret associate/disassociate failure.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorCode\"\n          },\n          \"description\": \"\\n            <p>Error code for associate/disassociate failure.</p>\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorMessage\"\n          },\n          \"description\": \"\\\
  n            <p>Error message for associate/disassociate failure.</p>\"\n        }\n      ]\n    },\n    \"SecretArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"secretArn\"\n          },\n          \"description\": \"\\n            <p>AWS Secrets Manager secret ARN.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-unprocessed-scram-secret-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UnprocessedScramSecret
---
