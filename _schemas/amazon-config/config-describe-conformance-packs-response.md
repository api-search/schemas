---
description: DescribeConformancePacksResponse schema
layout: schema
name: DescribeConformancePacksResponse
properties_list:
- description: ''
  name: ConformancePackDetails
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-conformance-packs-response-schema.json
slug: config-describe-conformance-packs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-packs-response-schema.json\",\n  \"title\": \"DescribeConformancePacksResponse\",\n  \"description\": \"DescribeConformancePacksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackDetailList\"\n        },\n        {\n          \"description\": \"Returns a list of <code>ConformancePackDetail</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response.\"\n      \
  \  }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-packs-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConformancePacksResponse
---
