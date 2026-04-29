---
description: Response from starting an investigation
layout: schema
name: StartInvestigationResponse
properties_list:
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-start-investigation-response-schema.json
slug: amazon-detective-start-investigation-response
source_filename: amazon-detective-start-investigation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-investigation-response-schema.json\",\n  \"title\": \"StartInvestigationResponse\",\n  \"description\": \"Response from starting an investigation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-investigation-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: StartInvestigationResponse
---
