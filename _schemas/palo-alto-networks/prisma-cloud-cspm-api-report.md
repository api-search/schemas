---
description: Report schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: Report
properties_list:
- description: Unique report identifier.
  name: id
  type: string
- description: Report name.
  name: name
  type: string
- description: Report type.
  name: type
  type: string
- description: Current report generation status.
  name: status
  type: string
- description: Epoch timestamp when the report was created.
  name: createdOn
  type: integer
- description: Epoch timestamp of last modification.
  name: lastModifiedOn
  type: integer
- description: URL for downloading the completed report.
  name: downloadUrl
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-report-schema.json
slug: prisma-cloud-cspm-api-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Report\",\n  \"description\": \"Report schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique report identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Report name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Report type.\",\n      \"enum\": [\n        \"RIS\",\n        \"COMPLIANCE\",\n        \"ALERT\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current report generation status.\"\
  \n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp when the report was created.\"\n    },\n    \"lastModifiedOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp of last modification.\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for downloading the completed report.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Report
---
