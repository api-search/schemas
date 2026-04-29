---
description: Certificate schema from Avalara API
layout: schema
name: Certificate
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: certificateNumber
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: signedDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: exemptionNumber
  type: string
- description: ''
  name: exemptionReason
  type: string
- description: ''
  name: exemptPercentage
  type: number
- description: Jurisdiction where the exemption applies
  name: exposureZone
  type: string
- description: ''
  name: customer
  type: object
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-certificate-schema.json
slug: certcapture-certificate
source_filename: certcapture-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-schema.json\",\n  \"title\": \"Certificate\",\n  \"description\": \"Certificate schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"certificateNumber\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Expired\",\n        \"Revoked\",\n        \"Pending\"\n      ]\n    },\n    \"signedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"exemptionNumber\": {\n      \"type\": \"string\"\n    },\n    \"exemptionReason\": {\n      \"type\": \"string\"\n    },\n    \"exemptPercentage\": {\n      \"type\": \"\
  number\",\n      \"format\": \"double\"\n    },\n    \"exposureZone\": {\n      \"type\": \"string\",\n      \"description\": \"Jurisdiction where the exemption applies\"\n    },\n    \"customer\": {\n      \"$ref\": \"#/components/schemas/CertCaptureCustomer\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-certificate-schema.json
tags:
- Taxes
title: Certificate
---
