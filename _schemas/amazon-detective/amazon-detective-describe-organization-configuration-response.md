---
description: Response from describing organization configuration
layout: schema
name: DescribeOrganizationConfigurationResponse
properties_list:
- description: Indicates whether to automatically enable new organization accounts as member accounts in the organization behavior graph.
  name: AutoEnable
  type: boolean
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-describe-organization-configuration-response-schema.json
slug: amazon-detective-describe-organization-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-describe-organization-configuration-response-schema.json\",\n  \"title\": \"DescribeOrganizationConfigurationResponse\",\n  \"description\": \"Response from describing organization configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether to automatically enable new organization accounts as member accounts in the organization behavior graph.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-describe-organization-configuration-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: DescribeOrganizationConfigurationResponse
---
