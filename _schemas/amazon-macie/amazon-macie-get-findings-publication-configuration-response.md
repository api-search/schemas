---
description: GetFindingsPublicationConfigurationResponse schema from Amazon Macie API
layout: schema
name: GetFindingsPublicationConfigurationResponse
properties_list:
- description: ''
  name: securityHubConfiguration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-findings-publication-configuration-response-schema.json
slug: amazon-macie-get-findings-publication-configuration-response
source_filename: amazon-macie-get-findings-publication-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-publication-configuration-response-schema.json\",\n  \"title\": \"GetFindingsPublicationConfigurationResponse\",\n  \"description\": \"GetFindingsPublicationConfigurationResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityHubConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityHubConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings that determine which findings are published to Security Hub.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-publication-configuration-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetFindingsPublicationConfigurationResponse
---
