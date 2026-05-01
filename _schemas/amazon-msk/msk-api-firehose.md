---
description: Firehose schema from Amazon MSK API
layout: schema
name: Firehose
properties_list:
- description: ''
  name: DeliveryStream
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-firehose-schema.json
slug: msk-api-firehose
source_filename: msk-api-firehose-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-firehose-schema.json\",\n  \"title\": \"Firehose\",\n  \"description\": \"Firehose schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deliveryStream\"\n          }\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-firehose-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Firehose
---
