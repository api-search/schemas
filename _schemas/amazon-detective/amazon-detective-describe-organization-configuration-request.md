---
description: Request to describe organization configuration
layout: schema
name: DescribeOrganizationConfigurationRequest
properties_list:
- description: The ARN of the organization behavior graph.
  name: GraphArn
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-describe-organization-configuration-request-schema.json
slug: amazon-detective-describe-organization-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-describe-organization-configuration-request-schema.json\",\n  \"title\": \"DescribeOrganizationConfigurationRequest\",\n  \"description\": \"Request to describe organization configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organization behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-describe-organization-configuration-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: DescribeOrganizationConfigurationRequest
---
