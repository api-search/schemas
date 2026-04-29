---
description: Information related to the software of the Sale System which manages the NEXO Sale to POI protocol.
layout: schema
name: SaleSoftware
properties_list:
- description: ''
  name: ManufacturerID
  type: string
- description: ''
  name: ApplicationName
  type: string
- description: ''
  name: SoftwareVersion
  type: string
- description: ''
  name: CertificationCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-software-schema.json
slug: terminal-sale-software
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-software-schema.json\",\n  \"title\": \"SaleSoftware\",\n  \"description\": \"Information related to the software of the Sale System which manages the NEXO Sale to POI protocol.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManufacturerID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"ApplicationName\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"SoftwareVersion\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"CertificationCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"ManufacturerID\",\n    \"ApplicationName\",\n    \"SoftwareVersion\",\n    \"CertificationCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-software-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleSoftware
---
