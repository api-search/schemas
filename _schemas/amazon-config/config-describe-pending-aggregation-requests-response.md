---
description: DescribePendingAggregationRequestsResponse schema
layout: schema
name: DescribePendingAggregationRequestsResponse
properties_list:
- description: ''
  name: PendingAggregationRequests
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-pending-aggregation-requests-response-schema.json
slug: config-describe-pending-aggregation-requests-response
source_filename: config-describe-pending-aggregation-requests-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-pending-aggregation-requests-response-schema.json\",\n  \"title\": \"DescribePendingAggregationRequestsResponse\",\n  \"description\": \"DescribePendingAggregationRequestsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PendingAggregationRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PendingAggregationRequestList\"\n        },\n        {\n          \"description\": \"Returns a PendingAggregationRequests object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-pending-aggregation-requests-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribePendingAggregationRequestsResponse
---
