---
description: UpdateOrganizationConfigurationResponse schema
layout: schema
name: UpdateOrganizationConfigurationResponse
properties_list:
- description: ''
  name: autoEnable
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-update-organization-configuration-response-schema.json
slug: inspector-update-organization-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-organization-configuration-response-schema.json\",\n  \"title\": \"UpdateOrganizationConfigurationResponse\",\n  \"description\": \"UpdateOrganizationConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoEnable\"\n        },\n        {\n          \"description\": \"The updated status of scan types automatically enabled for new members of your Amazon Inspector organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"autoEnable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-organization-configuration-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: UpdateOrganizationConfigurationResponse
---
