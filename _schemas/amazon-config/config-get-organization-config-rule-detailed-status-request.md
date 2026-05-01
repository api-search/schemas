---
description: GetOrganizationConfigRuleDetailedStatusRequest schema
layout: schema
name: GetOrganizationConfigRuleDetailedStatusRequest
properties_list:
- description: ''
  name: OrganizationConfigRuleName
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-organization-config-rule-detailed-status-request-schema.json
slug: config-get-organization-config-rule-detailed-status-request
source_filename: config-get-organization-config-rule-detailed-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-config-rule-detailed-status-request-schema.json\",\n  \"title\": \"GetOrganizationConfigRuleDetailedStatusRequest\",\n  \"description\": \"GetOrganizationConfigRuleDetailedStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of your organization Config rule for which you want status details for member accounts.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusDetailFilters\"\n        },\n        {\n          \"description\": \"A <code>StatusDetailFilters</code> object.\"\n        }\n\
  \      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CosmosPageLimit\"\n        },\n        {\n          \"description\": \"The maximum number of <code>OrganizationConfigRuleDetailedStatus</code> returned on each page. If you do not specify a number, Config uses the default. The default is 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-organization-config-rule-detailed-status-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetOrganizationConfigRuleDetailedStatusRequest
---
