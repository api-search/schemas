---
description: ''
layout: schema
name: GetReferenceResponse
properties_list:
- description: ''
  name: payload
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-reference-response-schema.json
slug: healthomics-get-reference-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-response-schema.json\",\n  \"title\": \"GetReferenceResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStreamingBlob\"\n        },\n        {\n          \"description\": \"The reference file payload.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetReferenceResponse
---
