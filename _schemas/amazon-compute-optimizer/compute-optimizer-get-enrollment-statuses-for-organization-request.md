---
description: GetEnrollmentStatusesForOrganizationRequest schema
layout: schema
name: GetEnrollmentStatusesForOrganizationRequest
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-enrollment-statuses-for-organization-request-schema.json
slug: compute-optimizer-get-enrollment-statuses-for-organization-request
source_filename: compute-optimizer-get-enrollment-statuses-for-organization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-statuses-for-organization-request-schema.json\",\n  \"title\": \"GetEnrollmentStatusesForOrganizationRequest\",\n  \"description\": \"GetEnrollmentStatusesForOrganizationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnrollmentFilters\"\n        },\n        {\n          \"description\": \"An array of objects to specify a filter that returns a more specific list of account enrollment statuses.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of account enrollment statuses.\"\
  \n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of account enrollment statuses to return with a single request. You can specify up to 100 statuses to return with each request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-statuses-for-organization-request-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEnrollmentStatusesForOrganizationRequest
---
