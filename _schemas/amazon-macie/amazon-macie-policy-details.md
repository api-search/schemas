---
description: Provides the details of a policy finding.
layout: schema
name: PolicyDetails
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: actor
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-policy-details-schema.json
slug: amazon-macie-policy-details
source_filename: amazon-macie-policy-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-policy-details-schema.json\",\n  \"title\": \"PolicyDetails\",\n  \"description\": \"Provides the details of a policy finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingAction\"\n        },\n        {\n          \"description\": \"The action that produced the finding.\"\n        }\n      ]\n    },\n    \"actor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingActor\"\n        },\n        {\n          \"description\": \"The entity that performed the action that produced the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-policy-details-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: PolicyDetails
---
