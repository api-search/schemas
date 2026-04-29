---
description: <p>Disassociates sasl scram secrets to cluster.</p>
layout: schema
name: BatchDisassociateScramSecretRequest
properties_list:
- description: ''
  name: SecretArnList
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-batch-disassociate-scram-secret-request-schema.json
slug: msk-api-batch-disassociate-scram-secret-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-batch-disassociate-scram-secret-request-schema.json\",\n  \"title\": \"BatchDisassociateScramSecretRequest\",\n  \"description\": \"\\n            <p>Disassociates sasl scram secrets to cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecretArnList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"secretArnList\"\n          },\n          \"description\": \"\\n            <p>List of AWS Secrets Manager secret ARNs.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SecretArnList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-batch-disassociate-scram-secret-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchDisassociateScramSecretRequest
---
