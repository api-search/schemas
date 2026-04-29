---
description: It conveys the result of the requested diagnosis and a possible message to display on a logical device. Content of the Diagnosis Response message.
layout: schema
name: DiagnosisResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: LoggedSaleID
  type: array
- description: ''
  name: POIStatus
  type: object
- description: ''
  name: HostStatus
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-diagnosis-response-schema.json
slug: terminal-diagnosis-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-diagnosis-response-schema.json\",\n  \"title\": \"DiagnosisResponse\",\n  \"description\": \"It conveys the result of the requested diagnosis and a possible message to display on a logical device. Content of the Diagnosis Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"LoggedSaleID\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^.+$\",\n        \"description\": \"If Sale Terminal logged to this POI Terminal.\"\n      }\n    },\n    \"POIStatus\": {\n      \"$ref\": \"#/components/schemas/POIStatus\"\n    },\n    \"HostStatus\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HostStatus\"\n      }\n\
  \    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-diagnosis-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DiagnosisResponse
---
