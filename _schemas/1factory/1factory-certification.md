---
description: Certification schema from 1Factory API
layout: schema
name: Certification
properties_list:
- description: Date and time when the certification expires.
  name: expiration_date
  type: string
- description: Name or type of the certification.
  name: certification
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-certification-schema.json
slug: 1factory-certification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-certification-schema.json\",\n  \"title\": \"Certification\",\n  \"description\": \"Certification schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": false,\n      \"description\": \"Date and time when the certification expires.\",\n      \"example\": \"2021-10-05T00:00:00-07:00\"\n    },\n    \"certification\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"maxLength\": 100,\n      \"description\": \"Name or type of the certification.\",\n      \"example\": \"ISO 9001\"\n    }\n  },\n  \"required\": [\n    \"expiration_date\",\n    \"certification\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-certification-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Certification
---
