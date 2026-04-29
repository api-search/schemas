---
description: Service health status information.
layout: schema
name: HealthStatus
properties_list:
- description: Overall service health status.
  name: status
  type: string
- description: Timestamp of the health check.
  name: timestamp
  type: string
- description: Current API version.
  name: version
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-health-status-schema.json
slug: moodys-data-buffet-health-status
source_filename: moodys-data-buffet-health-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HealthStatus\",\n  \"type\": \"object\",\n  \"description\": \"Service health status information.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall service health status.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the health check.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current API version.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-health-status-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: HealthStatus
---
