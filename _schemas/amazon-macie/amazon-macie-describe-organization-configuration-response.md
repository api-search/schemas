---
description: DescribeOrganizationConfigurationResponse schema from Amazon Macie API
layout: schema
name: DescribeOrganizationConfigurationResponse
properties_list:
- description: ''
  name: autoEnable
  type: object
- description: ''
  name: maxAccountLimitReached
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-describe-organization-configuration-response-schema.json
slug: amazon-macie-describe-organization-configuration-response
source_filename: amazon-macie-describe-organization-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-describe-organization-configuration-response-schema.json\",\n  \"title\": \"DescribeOrganizationConfigurationResponse\",\n  \"description\": \"DescribeOrganizationConfigurationResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon Macie is enabled automatically for accounts that are added to the organization.\"\n        }\n      ]\n    },\n    \"maxAccountLimitReached\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the maximum number of Amazon Macie member accounts\
  \ are part of the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-describe-organization-configuration-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DescribeOrganizationConfigurationResponse
---
