---
description: Specifies a severity level for findings that a custom data identifier produces. A severity level determines which severity is assigned to the findings, based on the number of occurrences of text that matches the custom data identifier's detection criteria.
layout: schema
name: SeverityLevel
properties_list:
- description: ''
  name: occurrencesThreshold
  type: object
- description: ''
  name: severity
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-severity-level-schema.json
slug: amazon-macie-severity-level
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-level-schema.json\",\n  \"title\": \"SeverityLevel\",\n  \"description\": \"Specifies a severity level for findings that a custom data identifier produces. A severity level determines which severity is assigned to the findings, based on the number of occurrences of text that matches the custom data identifier's detection criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"occurrencesThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The minimum number of occurrences of text that must match the custom data identifier's detection criteria in order to produce a finding with the specified severity (severity).\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DataIdentifierSeverity\"\n        },\n        {\n          \"description\": \"The severity to assign to a finding: if the number of occurrences is greater than or equal to the specified threshold (occurrencesThreshold); and, if applicable, the number of occurrences is less than the threshold for the next consecutive severity level for the custom data identifier, moving from LOW to HIGH.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"occurrencesThreshold\",\n    \"severity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-level-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SeverityLevel
---
