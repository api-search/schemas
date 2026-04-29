---
description: DescribeRemediationExecutionStatusResponse schema
layout: schema
name: DescribeRemediationExecutionStatusResponse
properties_list:
- description: ''
  name: RemediationExecutionStatuses
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-remediation-execution-status-response-schema.json
slug: config-describe-remediation-execution-status-response
source_filename: config-describe-remediation-execution-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-execution-status-response-schema.json\",\n  \"title\": \"DescribeRemediationExecutionStatusResponse\",\n  \"description\": \"DescribeRemediationExecutionStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RemediationExecutionStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationExecutionStatuses\"\n        },\n        {\n          \"description\": \"Returns a list of remediation execution statuses objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated\
  \ response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-remediation-execution-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeRemediationExecutionStatusResponse
---
