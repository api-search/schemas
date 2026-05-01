---
description: The request to update some combination of the Input Security Group name and the IPv4 CIDRs the Input Security Group should allow.
layout: schema
name: UpdateInputSecurityGroupRequest
properties_list:
- description: ''
  name: Tags
  type: object
- description: ''
  name: WhitelistRules
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-input-security-group-request-schema.json
slug: medialive-api-update-input-security-group-request
source_filename: medialive-api-update-input-security-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-security-group-request-schema.json\",\n  \"title\": \"UpdateInputSecurityGroupRequest\",\n  \"description\": \"The request to update some combination of the Input Security Group name and the IPv4 CIDRs the Input Security Group should allow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"WhitelistRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputWhitelistRuleCidr\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitelistRules\"\
  \n          },\n          \"description\": \"List of IPv4 CIDR addresses to whitelist\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-security-group-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateInputSecurityGroupRequest
---
