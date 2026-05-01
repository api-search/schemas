---
description: GetAggregateComplianceDetailsByConfigRuleRequest schema
layout: schema
name: GetAggregateComplianceDetailsByConfigRuleRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-compliance-details-by-config-rule-request-schema.json
slug: config-get-aggregate-compliance-details-by-config-rule-request
source_filename: config-get-aggregate-compliance-details-by-config-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-compliance-details-by-config-rule-request-schema.json\",\n  \"title\": \"GetAggregateComplianceDetailsByConfigRuleRequest\",\n  \"description\": \"GetAggregateComplianceDetailsByConfigRuleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule for which you want compliance information.\"\n        }\n      ]\n    },\n\
  \    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the source account.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region from where the data is aggregated.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"<p>The resource compliance status.</p> <note> <p>For the <code>GetAggregateComplianceDetailsByConfigRuleRequest</code> data type, Config supports only the <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>. Config does not support the <code>NOT_APPLICABLE</code> and <code>INSUFFICIENT_DATA</code> values.</p> </note>\"\n        }\n      ]\n\
  \    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of evaluation results returned on each page. The default is 50. You cannot specify a number greater than 100. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\",\n    \"ConfigRuleName\",\n    \"AccountId\",\n    \"AwsRegion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-compliance-details-by-config-rule-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateComplianceDetailsByConfigRuleRequest
---
