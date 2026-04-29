---
description: Unauthenticated schema from Amazon MSK API
layout: schema
name: Unauthenticated
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-unauthenticated-schema.json
slug: msk-api-unauthenticated
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-unauthenticated-schema.json\",\n  \"title\": \"Unauthenticated\",\n  \"description\": \"Unauthenticated schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          },\n          \"description\": \"\\n            <p>Specifies whether you want to turn on or turn off unauthenticated traffic to your cluster.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-unauthenticated-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Unauthenticated
---
