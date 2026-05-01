---
description: ListScramSecretsResponse schema from Amazon MSK API
layout: schema
name: ListScramSecretsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: SecretArnList
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-scram-secrets-response-schema.json
slug: msk-api-list-scram-secrets-response
source_filename: msk-api-list-scram-secrets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-scram-secrets-response-schema.json\",\n  \"title\": \"ListScramSecretsResponse\",\n  \"description\": \"ListScramSecretsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"\\n            <p>Paginated results marker.</p>\"\n        }\n      ]\n    },\n    \"SecretArnList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"secretArnList\"\n          },\n          \"description\": \"\\n            <p>The list of scram secrets\
  \ associated with the cluster.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-scram-secrets-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListScramSecretsResponse
---
