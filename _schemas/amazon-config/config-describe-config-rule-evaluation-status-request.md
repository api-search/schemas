---
description: <p/>
layout: schema
name: DescribeConfigRuleEvaluationStatusRequest
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-config-rule-evaluation-status-request-schema.json
slug: config-describe-config-rule-evaluation-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rule-evaluation-status-request-schema.json\",\n  \"title\": \"DescribeConfigRuleEvaluationStatusRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleNames\"\n        },\n        {\n          \"description\": \"The name of the Config managed rules for which you want status information. If you do not specify any names, Config returns status information for all Config managed rules that you use.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page\
  \ that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleLimit\"\n        },\n        {\n          \"description\": \"<p>The number of rule evaluation results that you want returned.</p> <p>This parameter is required if the rule limit for your account is more than the default of 150 rules.</p> <p>For information about requesting a rule limit increase, see <a href=\\\"http://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html#limits_config\\\">Config Limits</a> in the <i>Amazon Web Services General Reference Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-config-rule-evaluation-status-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigRuleEvaluationStatusRequest
---
