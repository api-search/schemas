---
description: Provides information about custom data identifiers that produced a sensitive data finding, and the number of occurrences of the data that they detected for the finding.
layout: schema
name: CustomDataIdentifiers
properties_list:
- description: ''
  name: detections
  type: object
- description: ''
  name: totalCount
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-custom-data-identifiers-schema.json
slug: amazon-macie-custom-data-identifiers
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-data-identifiers-schema.json\",\n  \"title\": \"CustomDataIdentifiers\",\n  \"description\": \"Provides information about custom data identifiers that produced a sensitive data finding, and the number of occurrences of the data that they detected for the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDetections\"\n        },\n        {\n          \"description\": \"The custom data identifiers that detected the data, and the number of occurrences of the data that each identifier detected.\"\n        }\n      ]\n    },\n    \"totalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\":\
  \ \"The total number of occurrences of the data that was detected by the custom data identifiers and produced the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-data-identifiers-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CustomDataIdentifiers
---
