---
description: S3 schema from Amazon MSK API
layout: schema
name: S3
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: Prefix
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-s3-schema.json
slug: msk-api-s3
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-s3-schema.json\",\n  \"title\": \"S3\",\n  \"description\": \"S3 schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bucket\"\n          }\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          }\n        }\n      ]\n    },\n    \"Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"prefix\"\n          }\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-s3-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: S3
---
