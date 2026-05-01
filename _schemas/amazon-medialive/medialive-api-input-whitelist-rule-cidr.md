---
description: An IPv4 CIDR to whitelist.
layout: schema
name: InputWhitelistRuleCidr
properties_list:
- description: ''
  name: Cidr
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-whitelist-rule-cidr-schema.json
slug: medialive-api-input-whitelist-rule-cidr
source_filename: medialive-api-input-whitelist-rule-cidr-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-whitelist-rule-cidr-schema.json\",\n  \"title\": \"InputWhitelistRuleCidr\",\n  \"description\": \"An IPv4 CIDR to whitelist.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cidr\"\n          },\n          \"description\": \"The IPv4 CIDR to whitelist.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-whitelist-rule-cidr-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputWhitelistRuleCidr
---
