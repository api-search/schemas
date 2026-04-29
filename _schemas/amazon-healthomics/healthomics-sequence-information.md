---
description: Details about a sequence.
layout: schema
name: SequenceInformation
properties_list:
- description: ''
  name: totalReadCount
  type: object
- description: ''
  name: totalBaseCount
  type: object
- description: ''
  name: generatedFrom
  type: object
- description: ''
  name: alignment
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-sequence-information-schema.json
slug: healthomics-sequence-information
source_filename: healthomics-sequence-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sequence-information-schema.json\",\n  \"title\": \"SequenceInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalReadCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The sequence's total read count.\"\n        }\n      ]\n    },\n    \"totalBaseCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The sequence's total base count.\"\n        }\n      ]\n    },\n    \"generatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedFrom\"\n        },\n        {\n          \"description\": \"Where the sequence originated.\"\n        }\n      ]\n  \
  \  },\n    \"alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The sequence's alignment setting.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details about a sequence.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sequence-information-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: SequenceInformation
---
