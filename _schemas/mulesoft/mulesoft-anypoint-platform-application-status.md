---
description: Detailed deployment status of a CloudHub application
layout: schema
name: ApplicationStatus
properties_list:
- description: Application domain name
  name: domain
  type: string
- description: Overall application status
  name: status
  type: string
- description: Status of the most recent deployment update
  name: deploymentUpdateStatus
  type: string
- description: ''
  name: workers
  type: array
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-application-status-schema.json
slug: mulesoft-anypoint-platform-application-status
source_filename: mulesoft-anypoint-platform-application-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationStatus\",\n  \"type\": \"object\",\n  \"description\": \"Detailed deployment status of a CloudHub application\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Application domain name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall application status\"\n    },\n    \"deploymentUpdateStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the most recent deployment update\"\n    },\n    \"workers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-application-status-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: ApplicationStatus
---
