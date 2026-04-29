---
description: Whitelist rule
layout: schema
name: InputWhitelistRule
properties_list:
- description: ''
  name: Cidr
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-whitelist-rule-schema.json
slug: medialive-api-input-whitelist-rule
source_filename: medialive-api-input-whitelist-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-whitelist-rule-schema.json\",\n  \"title\": \"InputWhitelistRule\",\n  \"description\": \"Whitelist rule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cidr\"\n          },\n          \"description\": \"The IPv4 CIDR that's whitelisted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-whitelist-rule-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputWhitelistRule
---
