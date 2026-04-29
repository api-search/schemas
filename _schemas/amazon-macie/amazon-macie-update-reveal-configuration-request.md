---
description: UpdateRevealConfigurationRequest schema from Amazon Macie API
layout: schema
name: UpdateRevealConfigurationRequest
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-reveal-configuration-request-schema.json
slug: amazon-macie-update-reveal-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-reveal-configuration-request-schema.json\",\n  \"title\": \"UpdateRevealConfigurationRequest\",\n  \"description\": \"UpdateRevealConfigurationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevealConfiguration\"\n        },\n        {\n          \"description\": \"The new configuration settings and the status of the configuration for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-reveal-configuration-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateRevealConfigurationRequest
---
