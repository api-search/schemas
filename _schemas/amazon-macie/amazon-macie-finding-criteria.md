---
description: Specifies, as a map, one or more property-based conditions that filter the results of a query for findings.
layout: schema
name: FindingCriteria
properties_list:
- description: ''
  name: criterion
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-criteria-schema.json
slug: amazon-macie-finding-criteria
source_filename: amazon-macie-finding-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-criteria-schema.json\",\n  \"title\": \"FindingCriteria\",\n  \"description\": \"Specifies, as a map, one or more property-based conditions that filter the results of a query for findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"criterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Criterion\"\n        },\n        {\n          \"description\": \"A condition that specifies the property, operator, and one or more values to use to filter the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingCriteria
---
