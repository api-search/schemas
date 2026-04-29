---
description: <p>Details for IAM access control.</p>
layout: schema
name: Iam
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-iam-schema.json
slug: msk-api-iam
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-iam-schema.json\",\n  \"title\": \"Iam\",\n  \"description\": \"\\n            <p>Details for IAM access control.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          },\n          \"description\": \"\\n            <p>Indicates whether IAM access control is enabled.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-iam-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Iam
---
