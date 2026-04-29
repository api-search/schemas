---
description: DescribeOrganizationConfigRuleStatusesRequest schema
layout: schema
name: DescribeOrganizationConfigRuleStatusesRequest
properties_list:
- description: ''
  name: OrganizationConfigRuleNames
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-organization-config-rule-statuses-request-schema.json
slug: config-describe-organization-config-rule-statuses-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-config-rule-statuses-request-schema.json\",\n  \"title\": \"DescribeOrganizationConfigRuleStatusesRequest\",\n  \"description\": \"DescribeOrganizationConfigRuleStatusesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleNames\"\n        },\n        {\n          \"description\": \"The names of organization Config rules for which you want status details. If you do not specify any names, Config returns details for all your organization Config rules.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CosmosPageLimit\"\n        },\n        {\n          \"description\"\
  : \"The maximum number of <code>OrganizationConfigRuleStatuses</code> returned on each page. If you do no specify a number, Config uses the default. The default is 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-organization-config-rule-statuses-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeOrganizationConfigRuleStatusesRequest
---
