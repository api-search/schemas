---
description: <p>Specifies the configuration to use for the brokers.</p>
layout: schema
name: ConfigurationInfo
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Revision
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-configuration-info-schema.json
slug: msk-api-configuration-info
source_filename: msk-api-configuration-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-info-schema.json\",\n  \"title\": \"ConfigurationInfo\",\n  \"description\": \"\\n            <p>Specifies the configuration to use for the brokers.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"\\n            <p>ARN of the configuration to use.</p>\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revision\"\n          },\n          \"description\": \"\\n            <p>The revision of the configuration to use.</p>\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Revision\",\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ConfigurationInfo
---
