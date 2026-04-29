---
description: DescribeOrganizationConfigurationResponse schema
layout: schema
name: DescribeOrganizationConfigurationResponse
properties_list:
- description: ''
  name: autoEnable
  type: object
- description: ''
  name: maxAccountLimitReached
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-describe-organization-configuration-response-schema.json
slug: inspector-describe-organization-configuration-response
source_filename: inspector-describe-organization-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-describe-organization-configuration-response-schema.json\",\n  \"title\": \"DescribeOrganizationConfigurationResponse\",\n  \"description\": \"DescribeOrganizationConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoEnable\"\n        },\n        {\n          \"description\": \"The scan types are automatically enabled for new members of your organization.\"\n        }\n      ]\n    },\n    \"maxAccountLimitReached\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Represents whether your organization has reached the maximum Amazon Web Services account limit for Amazon Inspector.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-describe-organization-configuration-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DescribeOrganizationConfigurationResponse
---
