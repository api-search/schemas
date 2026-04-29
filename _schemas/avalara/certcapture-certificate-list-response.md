---
description: CertificateListResponse schema from Avalara API
layout: schema
name: CertificateListResponse
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-certificate-list-response-schema.json
slug: certcapture-certificate-list-response
source_filename: certcapture-certificate-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-list-response-schema.json\",\n  \"title\": \"CertificateListResponse\",\n  \"description\": \"CertificateListResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Certificate\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-list-response-schema.json
tags:
- Taxes
title: CertificateListResponse
---
