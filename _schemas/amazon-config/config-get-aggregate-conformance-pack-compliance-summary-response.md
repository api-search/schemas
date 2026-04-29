---
description: GetAggregateConformancePackComplianceSummaryResponse schema
layout: schema
name: GetAggregateConformancePackComplianceSummaryResponse
properties_list:
- description: ''
  name: AggregateConformancePackComplianceSummaries
  type: object
- description: ''
  name: GroupByKey
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-conformance-pack-compliance-summary-response-schema.json
slug: config-get-aggregate-conformance-pack-compliance-summary-response
source_filename: config-get-aggregate-conformance-pack-compliance-summary-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-conformance-pack-compliance-summary-response-schema.json\",\n  \"title\": \"GetAggregateConformancePackComplianceSummaryResponse\",\n  \"description\": \"GetAggregateConformancePackComplianceSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggregateConformancePackComplianceSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateConformancePackComplianceSummaryList\"\n        },\n        {\n          \"description\": \"Returns a list of <code>AggregateConformancePackComplianceSummary</code> object.\"\n        }\n      ]\n    },\n    \"GroupByKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Groups the result\
  \ based on Amazon Web Services account ID or Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-conformance-pack-compliance-summary-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateConformancePackComplianceSummaryResponse
---
