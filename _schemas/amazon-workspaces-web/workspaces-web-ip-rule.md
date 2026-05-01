---
description: The IP rules of the IP access settings.
layout: schema
name: IpRule
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: ipRange
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-ip-rule-schema.json
slug: workspaces-web-ip-rule
source_filename: workspaces-web-ip-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ipRange\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the IP rule.\"\n        }\n      ]\n    },\n    \"ipRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRange\"\n        },\n        {\n          \"description\": \"The IP range of the IP rule.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The IP rules of the IP access settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-rule-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IpRule
---
