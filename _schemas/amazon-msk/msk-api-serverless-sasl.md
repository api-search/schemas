---
description: <p>Details for client authentication using SASL.</p>
layout: schema
name: ServerlessSasl
properties_list:
- description: ''
  name: Iam
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-serverless-sasl-schema.json
slug: msk-api-serverless-sasl
source_filename: msk-api-serverless-sasl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-sasl-schema.json\",\n  \"title\": \"ServerlessSasl\",\n  \"description\": \"\\n            <p>Details for client authentication using SASL.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Iam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Iam\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iam\"\n          },\n          \"description\": \"\\n            <p>Indicates whether IAM access control is enabled.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-sasl-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ServerlessSasl
---
