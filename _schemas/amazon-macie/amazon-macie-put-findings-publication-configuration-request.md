---
description: PutFindingsPublicationConfigurationRequest schema from Amazon Macie API
layout: schema
name: PutFindingsPublicationConfigurationRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: securityHubConfiguration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-put-findings-publication-configuration-request-schema.json
slug: amazon-macie-put-findings-publication-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-put-findings-publication-configuration-request-schema.json\",\n  \"title\": \"PutFindingsPublicationConfigurationRequest\",\n  \"description\": \"PutFindingsPublicationConfigurationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"securityHubConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityHubConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings that determine which findings to publish\
  \ to Security Hub.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-put-findings-publication-configuration-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: PutFindingsPublicationConfigurationRequest
---
