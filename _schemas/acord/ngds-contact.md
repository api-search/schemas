---
description: Contact schema from ACORD NGDS API
layout: schema
name: Contact
properties_list:
- description: ''
  name: contactType
  type: string
- description: ''
  name: value
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-contact-schema.json
slug: ngds-contact
source_filename: ngds-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Phone\",\n        \"Email\",\n        \"Fax\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-contact-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: Contact
---
