---
description: DescribeAggregateComplianceByConformancePacksRequest schema
layout: schema
name: DescribeAggregateComplianceByConformancePacksRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
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
schema_file: json-schema/config-describe-aggregate-compliance-by-conformance-packs-request-schema.json
slug: config-describe-aggregate-compliance-by-conformance-packs-request
source_filename: config-describe-aggregate-compliance-by-conformance-packs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregate-compliance-by-conformance-packs-request-schema.json\",\n  \"title\": \"DescribeAggregateComplianceByConformancePacksRequest\",\n  \"description\": \"DescribeAggregateComplianceByConformancePacksRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateConformancePackComplianceFilters\"\n        },\n        {\n          \"description\": \"Filters the result by <code>AggregateConformancePackComplianceFilters</code>\
  \ object.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of conformance packs compliance details returned on each page. The default is maximum. If you specify 0, Config uses the default. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-aggregate-compliance-by-conformance-packs-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeAggregateComplianceByConformancePacksRequest
---
