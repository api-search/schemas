---
description: GetAggregateConformancePackComplianceSummaryRequest schema
layout: schema
name: GetAggregateConformancePackComplianceSummaryRequest
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
schema_file: json-schema/config-get-aggregate-conformance-pack-compliance-summary-request-schema.json
slug: config-get-aggregate-conformance-pack-compliance-summary-request
source_filename: config-get-aggregate-conformance-pack-compliance-summary-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-conformance-pack-compliance-summary-request-schema.json\",\n  \"title\": \"GetAggregateConformancePackComplianceSummaryRequest\",\n  \"description\": \"GetAggregateConformancePackComplianceSummaryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateConformancePackComplianceSummaryFilters\"\n        },\n        {\n          \"description\": \"Filters the results based on the <code>AggregateConformancePackComplianceSummaryFilters</code>\
  \ object.\"\n        }\n      ]\n    },\n    \"GroupByKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateConformancePackComplianceSummaryGroupKey\"\n        },\n        {\n          \"description\": \"Groups the result based on Amazon Web Services account ID or Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of results returned on each page. The default is maximum. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-conformance-pack-compliance-summary-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateConformancePackComplianceSummaryRequest
---
