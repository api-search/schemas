---
description: <p>Details for client authentication using SASL.</p>
layout: schema
name: Sasl
properties_list:
- description: ''
  name: Scram
  type: object
- description: ''
  name: Iam
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-sasl-schema.json
slug: msk-api-sasl
source_filename: msk-api-sasl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-sasl-schema.json\",\n  \"title\": \"Sasl\",\n  \"description\": \"\\n            <p>Details for client authentication using SASL.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Scram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scram\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scram\"\n          },\n          \"description\": \"\\n            <p>Details for SASL/SCRAM client authentication.</p>\"\n        }\n      ]\n    },\n    \"Iam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Iam\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iam\"\n          },\n          \"description\": \"\\n            <p>Indicates whether IAM access control is enabled.</p>\"\n        }\n   \
  \   ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-sasl-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Sasl
---
