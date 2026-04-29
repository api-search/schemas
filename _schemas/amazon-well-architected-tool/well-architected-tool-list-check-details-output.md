---
description: ListCheckDetailsOutput schema from AWS Well-Architected Tool API
layout: schema
name: ListCheckDetailsOutput
properties_list:
- description: ''
  name: CheckDetails
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-check-details-output-schema.json
slug: well-architected-tool-list-check-details-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CheckDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckDetails\"\n        },\n        {\n          \"description\": \"The details about the Trusted Advisor checks related to the Well-Architected best practice.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListCheckDetailsOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-check-details-output-schema.json\",\n  \"description\": \"ListCheckDetailsOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-check-details-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListCheckDetailsOutput
---
