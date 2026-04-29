---
description: DownloadCsvRequest schema from Incident Security Service Posture Management API
layout: schema
name: DownloadCsvRequest
properties_list:
- description: ''
  name: userFullName
  type: string
- description: ''
  name: userEmail
  type: string
- description: ''
  name: service
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-download-csv-request-schema.json
slug: identity-security-posture-management-api-download-csv-request
source_filename: identity-security-posture-management-api-download-csv-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DownloadCsvRequest\",\n  \"description\": \"DownloadCsvRequest schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-download-csv-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userFullName\": {\n      \"type\": \"string\"\n    },\n    \"userEmail\": {\n      \"type\": \"string\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"userFullName\",\n    \"userEmail\",\n    \"service\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-download-csv-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DownloadCsvRequest
---
