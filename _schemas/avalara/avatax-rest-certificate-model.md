---
description: CertificateModel schema from Avalara API
layout: schema
name: CertificateModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: companyId
  type: integer
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
  name: exemptPercentage
  type: number
- description: ''
  name: exemptionReason
  type: object
- description: ''
  name: status
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-certificate-model-schema.json
slug: avatax-rest-certificate-model
source_filename: avatax-rest-certificate-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-certificate-model-schema.json\",\n  \"title\": \"CertificateModel\",\n  \"description\": \"CertificateModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\"\n    },\n    \"signedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"exemptionNumber\": {\n      \"type\": \"string\"\n    },\n    \"exemptPercentage\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"exemptionReason\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n        \
  \  \"type\": \"string\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-certificate-model-schema.json
tags:
- Taxes
title: CertificateModel
---
