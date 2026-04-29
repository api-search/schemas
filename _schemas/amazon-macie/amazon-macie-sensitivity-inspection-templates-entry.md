---
description: Provides information about the sensitivity inspection template for an Amazon Macie account. Macie uses the template's settings when it performs automated sensitive data discovery for the account.
layout: schema
name: SensitivityInspectionTemplatesEntry
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitivity-inspection-templates-entry-schema.json
slug: amazon-macie-sensitivity-inspection-templates-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-templates-entry-schema.json\",\n  \"title\": \"SensitivityInspectionTemplatesEntry\",\n  \"description\": \"Provides information about the sensitivity inspection template for an Amazon Macie account. Macie uses the template's settings when it performs automated sensitive data discovery for the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the sensitivity inspection template.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the sensitivity\
  \ inspection template: automated-sensitive-data-discovery.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-templates-entry-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitivityInspectionTemplatesEntry
---
