---
description: DescribeConformancePackStatusResponse schema
layout: schema
name: DescribeConformancePackStatusResponse
properties_list:
- description: ''
  name: ConformancePackStatusDetails
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-conformance-pack-status-response-schema.json
slug: config-describe-conformance-pack-status-response
source_filename: config-describe-conformance-pack-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-status-response-schema.json\",\n  \"title\": \"DescribeConformancePackStatusResponse\",\n  \"description\": \"DescribeConformancePackStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackStatusDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackStatusDetailsList\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackStatusDetail</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated\
  \ response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-status-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConformancePackStatusResponse
---
