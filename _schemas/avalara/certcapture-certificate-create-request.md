---
description: CertificateCreateRequest schema from Avalara API
layout: schema
name: CertificateCreateRequest
properties_list:
- description: ''
  name: exemptionNumber
  type: string
- description: ''
  name: exemptionReason
  type: string
- description: ''
  name: exposureZone
  type: string
- description: ''
  name: signedDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: exemptPercentage
  type: number
- description: ''
  name: customerCode
  type: string
- description: ''
  name: attributes
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-certificate-create-request-schema.json
slug: certcapture-certificate-create-request
source_filename: certcapture-certificate-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-create-request-schema.json\",\n  \"title\": \"CertificateCreateRequest\",\n  \"description\": \"CertificateCreateRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"exemptionReason\",\n    \"exposureZone\"\n  ],\n  \"properties\": {\n    \"exemptionNumber\": {\n      \"type\": \"string\"\n    },\n    \"exemptionReason\": {\n      \"type\": \"string\"\n    },\n    \"exposureZone\": {\n      \"type\": \"string\"\n    },\n    \"signedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"exemptPercentage\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"customerCode\": {\n      \"type\": \"string\"\n    },\n  \
  \  \"attributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CertAttribute\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-create-request-schema.json
tags:
- Taxes
title: CertificateCreateRequest
---
