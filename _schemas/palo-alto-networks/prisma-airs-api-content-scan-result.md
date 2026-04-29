---
description: ContentScanResult schema from Palo Alto Networks Prisma AIRS API
layout: schema
name: ContentScanResult
properties_list:
- description: Threats detected in the prompt field.
  name: prompt_detected
  type: object
- description: Threats detected in the response field.
  name: response_detected
  type: object
- description: Overall verdict for this content pair.
  name: verdict
  type: string
- description: Action taken based on the security profile configuration.
  name: action
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-airs-api-content-scan-result-schema.json
slug: prisma-airs-api-content-scan-result
source_filename: prisma-airs-api-content-scan-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentScanResult\",\n  \"description\": \"ContentScanResult schema from Palo Alto Networks Prisma AIRS API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-content-scan-result-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_detected\": {\n      \"type\": \"object\",\n      \"description\": \"Threats detected in the prompt field.\",\n      \"properties\": {\n        \"url_cats\": {\n          \"type\": \"boolean\",\n          \"description\": \"Malicious URL categories detected in prompt.\"\n        },\n        \"dlp\": {\n          \"type\": \"boolean\",\n          \"description\": \"Data loss prevention triggers in prompt.\"\n        },\n        \"injection\": {\n          \"type\": \"boolean\",\n          \"description\": \"Prompt injection detected.\"\n        }\n      }\n    },\n \
  \   \"response_detected\": {\n      \"type\": \"object\",\n      \"description\": \"Threats detected in the response field.\",\n      \"properties\": {\n        \"url_cats\": {\n          \"type\": \"boolean\",\n          \"description\": \"Malicious URL categories detected in response.\"\n        },\n        \"dlp\": {\n          \"type\": \"boolean\",\n          \"description\": \"Data loss prevention triggers in response.\"\n        },\n        \"toxic_content\": {\n          \"type\": \"boolean\",\n          \"description\": \"Toxic or harmful content detected in response.\"\n        }\n      }\n    },\n    \"verdict\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"benign\",\n        \"malicious\"\n      ],\n      \"description\": \"Overall verdict for this content pair.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"block\"\n      ],\n      \"description\": \"Action taken based on the security profile configuration.\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-airs-api-content-scan-result-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ContentScanResult
---
