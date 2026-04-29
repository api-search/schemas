---
description: It conveys Information related to the target POI for which the diagnosis is requested. Content of the Diagnosis Request message.
layout: schema
name: DiagnosisRequest
properties_list:
- description: MessageHeader.POIID.
  name: POIID
  type: string
- description: Indicates if Host Diagnosis are required.
  name: HostDiagnosisFlag
  type: boolean
- description: ''
  name: AcquirerID
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-diagnosis-request-schema.json
slug: terminal-diagnosis-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-diagnosis-request-schema.json\",\n  \"title\": \"DiagnosisRequest\",\n  \"description\": \"It conveys Information related to the target POI for which the diagnosis is requested. Content of the Diagnosis Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"MessageHeader.POIID.\"\n    },\n    \"HostDiagnosisFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Indicates if Host Diagnosis are required.\"\n    },\n    \"AcquirerID\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"description\": \"Present if requesting the diagnosis of these hosts only.\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-diagnosis-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DiagnosisRequest
---
