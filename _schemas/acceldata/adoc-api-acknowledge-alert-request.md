---
description: Request body for acknowledging an alert
layout: schema
name: AcknowledgeAlertRequest
properties_list:
- description: Optional comment explaining the acknowledgement
  name: comment
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-acknowledge-alert-request-schema.json
slug: adoc-api-acknowledge-alert-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/acknowledge-alert-request.json\",\n  \"title\": \"AcknowledgeAlertRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for acknowledging an alert\",\n  \"properties\": {\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment explaining the acknowledgement\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-acknowledge-alert-request-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: AcknowledgeAlertRequest
---
