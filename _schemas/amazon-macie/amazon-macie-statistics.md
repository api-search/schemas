---
description: Provides processing statistics for a classification job.
layout: schema
name: Statistics
properties_list:
- description: ''
  name: approximateNumberOfObjectsToProcess
  type: object
- description: ''
  name: numberOfRuns
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-statistics-schema.json
slug: amazon-macie-statistics
source_filename: amazon-macie-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-statistics-schema.json\",\n  \"title\": \"Statistics\",\n  \"description\": \"Provides processing statistics for a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"approximateNumberOfObjectsToProcess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The approximate number of objects that the job has yet to process during its current run.\"\n        }\n      ]\n    },\n    \"numberOfRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The number of times that the job has run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-statistics-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Statistics
---
