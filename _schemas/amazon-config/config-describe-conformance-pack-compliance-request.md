---
description: DescribeConformancePackComplianceRequest schema
layout: schema
name: DescribeConformancePackComplianceRequest
properties_list:
- description: ''
  name: ConformancePackName
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
schema_file: json-schema/config-describe-conformance-pack-compliance-request-schema.json
slug: config-describe-conformance-pack-compliance-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-compliance-request-schema.json\",\n  \"title\": \"DescribeConformancePackComplianceRequest\",\n  \"description\": \"DescribeConformancePackComplianceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceFilters\"\n        },\n        {\n          \"description\": \"A <code>ConformancePackComplianceFilters</code> object.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/DescribeConformancePackComplianceLimit\"\n        },\n        {\n          \"description\": \"The maximum number of Config rules within a conformance pack are returned on each page.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned in a previous request that you use to request the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-conformance-pack-compliance-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConformancePackComplianceRequest
---
