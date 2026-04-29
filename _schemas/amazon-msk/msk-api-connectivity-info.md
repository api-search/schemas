---
description: <p>Information about the broker access configuration.</p>
layout: schema
name: ConnectivityInfo
properties_list:
- description: ''
  name: PublicAccess
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-connectivity-info-schema.json
slug: msk-api-connectivity-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-connectivity-info-schema.json\",\n  \"title\": \"ConnectivityInfo\",\n  \"description\": \"\\n            <p>Information about the broker access configuration.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicAccess\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publicAccess\"\n          },\n          \"description\": \"\\n            <p>Public access control for brokers.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-connectivity-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConnectivityInfo
---
