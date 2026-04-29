---
description: CertAttribute schema from Avalara API
layout: schema
name: CertAttribute
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: isSystemCode
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-cert-attribute-schema.json
slug: certcapture-cert-attribute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-cert-attribute-schema.json\",\n  \"title\": \"CertAttribute\",\n  \"description\": \"CertAttribute schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"isSystemCode\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-cert-attribute-schema.json
tags:
- Taxes
title: CertAttribute
---
