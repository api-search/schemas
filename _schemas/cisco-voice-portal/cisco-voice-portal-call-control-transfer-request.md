---
description: ''
layout: schema
name: TransferRequest
properties_list:
- description: Transfer destination (phone number, SIP URI, or agent extension)
  name: destination
  type: string
- description: Type of transfer
  name: transferType
  type: string
- description: ICM label for the transfer destination. Used when routing through ICM/UCCE.
  name: label
  type: string
- description: ECC variables to pass with the transfer
  name: eccVariables
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-transfer-request-schema.json
slug: cisco-voice-portal-call-control-transfer-request
source_filename: cisco-voice-portal-call-control-transfer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransferRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Transfer destination (phone number, SIP URI, or agent extension)\"\n    },\n    \"transferType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of transfer\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"ICM label for the transfer destination. Used when routing through ICM/UCCE.\"\n    },\n    \"eccVariables\": {\n      \"type\": \"object\",\n      \"description\": \"ECC variables to pass with the transfer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-transfer-request-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: TransferRequest
---
