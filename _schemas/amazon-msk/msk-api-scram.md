---
description: <p>Details for SASL/SCRAM client authentication.</p>
layout: schema
name: Scram
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-scram-schema.json
slug: msk-api-scram
source_filename: msk-api-scram-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-scram-schema.json\",\n  \"title\": \"Scram\",\n  \"description\": \"\\n            <p>Details for SASL/SCRAM client authentication.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          },\n          \"description\": \"\\n            <p>SASL/SCRAM authentication is enabled or not.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-scram-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scram
---
