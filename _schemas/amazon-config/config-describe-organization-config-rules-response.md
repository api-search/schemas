---
description: DescribeOrganizationConfigRulesResponse schema
layout: schema
name: DescribeOrganizationConfigRulesResponse
properties_list:
- description: ''
  name: OrganizationConfigRules
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-organization-config-rules-response-schema.json
slug: config-describe-organization-config-rules-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-config-rules-response-schema.json\",\n  \"title\": \"DescribeOrganizationConfigRulesResponse\",\n  \"description\": \"DescribeOrganizationConfigRulesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRules\"\n        },\n        {\n          \"description\": \"Returns a list of <code>OrganizationConfigRule</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\
  \ \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-config-rules-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeOrganizationConfigRulesResponse
---
