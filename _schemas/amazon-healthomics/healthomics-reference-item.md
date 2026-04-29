---
description: A genome reference.
layout: schema
name: ReferenceItem
properties_list:
- description: ''
  name: referenceArn
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-reference-item-schema.json
slug: healthomics-reference-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-item-schema.json\",\n  \"title\": \"ReferenceItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"referenceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \"The reference's ARN.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A genome reference.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReferenceItem
---
