---
description: Request to update organization configuration
layout: schema
name: UpdateOrganizationConfigurationRequest
properties_list:
- description: The ARN of the organization behavior graph.
  name: GraphArn
  type: string
- description: Indicates whether to automatically enable new organization accounts as member accounts in the organization behavior graph.
  name: AutoEnable
  type: boolean
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-update-organization-configuration-request-schema.json
slug: amazon-detective-update-organization-configuration-request
source_filename: amazon-detective-update-organization-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-organization-configuration-request-schema.json\",\n  \"title\": \"UpdateOrganizationConfigurationRequest\",\n  \"description\": \"Request to update organization configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organization behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"AutoEnable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether to automatically enable new organization accounts as member accounts in the organization behavior graph.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-organization-configuration-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: UpdateOrganizationConfigurationRequest
---
