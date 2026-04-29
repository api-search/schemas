---
description: LocalizedString from LinkedIn API
layout: schema
name: LocalizedString
properties_list:
- description: ''
  name: localized
  type: object
- description: ''
  name: preferredLocale
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-localized-string-schema.json
slug: linkedin-regulations-data-portability-localized-string
source_filename: linkedin-regulations-data-portability-localized-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-localized-string-schema.json\",\n  \"title\": \"LocalizedString\",\n  \"description\": \"LocalizedString from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"localized\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"en_US\": \"Acme Corporation\"\n      }\n    },\n    \"preferredLocale\": {\n      \"$ref\": \"#/components/schemas/Locale\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-localized-string-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: LocalizedString
---
