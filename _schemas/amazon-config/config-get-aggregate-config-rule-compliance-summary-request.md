---
description: GetAggregateConfigRuleComplianceSummaryRequest schema
layout: schema
name: GetAggregateConfigRuleComplianceSummaryRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: GroupByKey
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-config-rule-compliance-summary-request-schema.json
slug: config-get-aggregate-config-rule-compliance-summary-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-config-rule-compliance-summary-request-schema.json\",\n  \"title\": \"GetAggregateConfigRuleComplianceSummaryRequest\",\n  \"description\": \"GetAggregateConfigRuleComplianceSummaryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleComplianceSummaryFilters\"\n        },\n        {\n          \"description\": \"Filters the results based on the ConfigRuleComplianceSummaryFilters object.\"\n        }\n   \
  \   ]\n    },\n    \"GroupByKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleComplianceSummaryGroupKey\"\n        },\n        {\n          \"description\": \"Groups the result based on ACCOUNT_ID or AWS_REGION.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupByAPILimit\"\n        },\n        {\n          \"description\": \"The maximum number of evaluation results returned on each page. The default is 1000. You cannot specify a number greater than 1000. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-config-rule-compliance-summary-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateConfigRuleComplianceSummaryRequest
---
