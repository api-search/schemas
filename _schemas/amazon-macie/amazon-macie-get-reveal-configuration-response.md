---
description: GetRevealConfigurationResponse schema from Amazon Macie API
layout: schema
name: GetRevealConfigurationResponse
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-reveal-configuration-response-schema.json
slug: amazon-macie-get-reveal-configuration-response
source_filename: amazon-macie-get-reveal-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-reveal-configuration-response-schema.json\",\n  \"title\": \"GetRevealConfigurationResponse\",\n  \"description\": \"GetRevealConfigurationResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevealConfiguration\"\n        },\n        {\n          \"description\": \"The current configuration settings and the status of the configuration for the account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-reveal-configuration-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetRevealConfigurationResponse
---
