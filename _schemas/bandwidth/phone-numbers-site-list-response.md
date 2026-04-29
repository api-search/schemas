---
description: Response containing a list of sites
layout: schema
name: SiteListResponse
properties_list:
- description: ''
  name: sites
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-site-list-response-schema.json
slug: phone-numbers-site-list-response
source_filename: phone-numbers-site-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-site-list-response-schema.json\",\n  \"title\": \"SiteListResponse\",\n  \"description\": \"Response containing a list of sites\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sites\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Site\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-site-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: SiteListResponse
---
