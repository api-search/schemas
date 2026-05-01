---
description: DescribeRemediationExecutionStatusRequest schema
layout: schema
name: DescribeRemediationExecutionStatusRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ResourceKeys
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-remediation-execution-status-request-schema.json
slug: config-describe-remediation-execution-status-request
source_filename: config-describe-remediation-execution-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-execution-status-request-schema.json\",\n  \"title\": \"DescribeRemediationExecutionStatusRequest\",\n  \"description\": \"DescribeRemediationExecutionStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"A list of Config rule names.\"\n        }\n      ]\n    },\n    \"ResourceKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceKeys\"\n        },\n        {\n          \"description\": \"A list of resource keys to be processed with the current request. Each element in the list consists of the resource type and resource ID. \"\n        }\n      ]\n    },\n\
  \    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of RemediationExecutionStatuses returned on each page. The default is maximum. If you specify 0, Config uses the default. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-execution-status-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeRemediationExecutionStatusRequest
---
