---
description: DescribePendingAggregationRequestsRequest schema
layout: schema
name: DescribePendingAggregationRequestsRequest
properties_list:
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-pending-aggregation-requests-request-schema.json
slug: config-describe-pending-aggregation-requests-request
source_filename: config-describe-pending-aggregation-requests-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-pending-aggregation-requests-request-schema.json\",\n  \"title\": \"DescribePendingAggregationRequestsRequest\",\n  \"description\": \"DescribePendingAggregationRequestsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribePendingAggregationRequestsLimit\"\n        },\n        {\n          \"description\": \"The maximum number of evaluation results returned on each page. The default is maximum. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page\
  \ that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-pending-aggregation-requests-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribePendingAggregationRequestsRequest
---
