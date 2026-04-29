---
description: DescribeConformancePacksRequest schema
layout: schema
name: DescribeConformancePacksRequest
properties_list:
- description: ''
  name: ConformancePackNames
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-conformance-packs-request-schema.json
slug: config-describe-conformance-packs-request
source_filename: config-describe-conformance-packs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-packs-request-schema.json\",\n  \"title\": \"DescribeConformancePacksRequest\",\n  \"description\": \"DescribeConformancePacksRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackNamesList\"\n        },\n        {\n          \"description\": \"Comma-separated list of conformance pack names for which you want details. If you do not specify any names, Config returns details for all your conformance packs. \"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSizeLimit\"\n        },\n        {\n          \"description\": \"The maximum number of conformance packs returned on each\
  \ page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-packs-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConformancePacksRequest
---
