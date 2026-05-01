---
description: Response from listing investigations
layout: schema
name: ListInvestigationsResponse
properties_list:
- description: Lists the summary of uncommon behavior or malicious activity which indicates a compromise.
  name: InvestigationDetails
  type: array
- description: Lists investigations for a behavior graph based on the maximum number of investigations in a page.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-investigations-response-schema.json
slug: amazon-detective-list-investigations-response
source_filename: amazon-detective-list-investigations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-investigations-response-schema.json\",\n  \"title\": \"ListInvestigationsResponse\",\n  \"description\": \"Response from listing investigations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvestigationDetails\": {\n      \"type\": \"array\",\n      \"description\": \"Lists the summary of uncommon behavior or malicious activity which indicates a compromise.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvestigationDetail\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Lists investigations for a behavior graph based on the maximum number of investigations in a page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-investigations-response-schema.json
tags:
- Forensics
- Investigation
- Security
title: ListInvestigationsResponse
---
