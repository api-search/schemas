---
description: GetSensitivityInspectionTemplateResponse schema from Amazon Macie API
layout: schema
name: GetSensitivityInspectionTemplateResponse
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: excludes
  type: object
- description: ''
  name: includes
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: sensitivityInspectionTemplateId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-sensitivity-inspection-template-response-schema.json
slug: amazon-macie-get-sensitivity-inspection-template-response
source_filename: amazon-macie-get-sensitivity-inspection-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-sensitivity-inspection-template-response-schema.json\",\n  \"title\": \"GetSensitivityInspectionTemplateResponse\",\n  \"description\": \"GetSensitivityInspectionTemplateResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the template.\"\n        }\n      ]\n    },\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateExcludes\"\n        },\n        {\n          \"description\": \" <p>The managed data identifiers that are explicitly excluded (not used) when analyzing data.</p>\"\n        }\n      ]\n\
  \    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateIncludes\"\n        },\n        {\n          \"description\": \"The allow lists, custom data identifiers, and managed data identifiers that are included (used) when analyzing data.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the template: automated-sensitive-data-discovery.\"\n        }\n      ]\n    },\n    \"sensitivityInspectionTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateId\"\n        },\n        {\n          \"description\": \"The unique identifier for the template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-sensitivity-inspection-template-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetSensitivityInspectionTemplateResponse
---
