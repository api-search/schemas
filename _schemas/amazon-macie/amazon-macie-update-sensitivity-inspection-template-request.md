---
description: UpdateSensitivityInspectionTemplateRequest schema from Amazon Macie API
layout: schema
name: UpdateSensitivityInspectionTemplateRequest
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
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-sensitivity-inspection-template-request-schema.json
slug: amazon-macie-update-sensitivity-inspection-template-request
source_filename: amazon-macie-update-sensitivity-inspection-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-sensitivity-inspection-template-request-schema.json\",\n  \"title\": \"UpdateSensitivityInspectionTemplateRequest\",\n  \"description\": \"UpdateSensitivityInspectionTemplateRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A custom description of the template. The description can contain as many as 200 characters.\"\n        }\n      ]\n    },\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateExcludes\"\n        },\n        {\n          \"description\": \" <p>The managed data identifiers to explicitly exclude (not use)\
  \ when analyzing data.</p> <p>To exclude an allow list or custom data identifier that's currently included by the template, update the values for the SensitivityInspectionTemplateIncludes.allowListIds and SensitivityInspectionTemplateIncludes.customDataIdentifierIds properties, respectively.</p>\"\n        }\n      ]\n    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateIncludes\"\n        },\n        {\n          \"description\": \"The allow lists, custom data identifiers, and managed data identifiers to include (use) when analyzing data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-sensitivity-inspection-template-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateSensitivityInspectionTemplateRequest
---
