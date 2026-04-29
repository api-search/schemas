---
description: UpdateOrganizationConfigurationRequest schema from Amazon Macie API
layout: schema
name: UpdateOrganizationConfigurationRequest
properties_list:
- description: ''
  name: autoEnable
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-organization-configuration-request-schema.json
slug: amazon-macie-update-organization-configuration-request
source_filename: amazon-macie-update-organization-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-organization-configuration-request-schema.json\",\n  \"title\": \"UpdateOrganizationConfigurationRequest\",\n  \"description\": \"UpdateOrganizationConfigurationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable Amazon Macie automatically for an account when the account is added to the organization in Organizations.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"autoEnable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-organization-configuration-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateOrganizationConfigurationRequest
---
