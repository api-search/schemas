---
description: Client information mapping with source system identifiers
layout: schema
name: SourceSystemClientMapping
properties_list:
- description: Source system Client unique ID created and managed by institution system. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: clientId
  type: string
- description: Client unique Reference Number created and managed by institution CBS. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: cbsReferenceNumber
  type: string
- description: Client unique ID created and managed by institution CBS.
  name: cbsClientId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-source-system-client-mapping-schema.json
slug: mastercard-card-issuance-source-system-client-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SourceSystemClientMapping\",\n  \"type\": \"object\",\n  \"description\": \"Client information mapping with source system identifiers\",\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Source system Client unique ID created and managed by institution system. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"cbsReferenceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Client unique Reference Number created and managed by institution CBS. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"cbsClientId\": {\n      \"type\": \"string\",\n      \"description\": \"Client unique ID created and managed by institution CBS.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-source-system-client-mapping-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SourceSystemClientMapping
---
