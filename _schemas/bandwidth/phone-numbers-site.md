---
description: A site (sub-account) within a Bandwidth account
layout: schema
name: Site
properties_list:
- description: The unique identifier for the site
  name: id
  type: string
- description: The name of the site
  name: name
  type: string
- description: A description of the site
  name: description
  type: string
- description: ''
  name: address
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-site-schema.json
slug: phone-numbers-site
source_filename: phone-numbers-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-site-schema.json\",\n  \"title\": \"Site\",\n  \"description\": \"A site (sub-account) within a Bandwidth account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the site\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the site\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the site\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-site-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Site
---
