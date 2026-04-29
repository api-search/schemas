---
description: GetEnrollmentStatusesForOrganizationResponse schema
layout: schema
name: GetEnrollmentStatusesForOrganizationResponse
properties_list:
- description: ''
  name: accountEnrollmentStatuses
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-enrollment-statuses-for-organization-response-schema.json
slug: compute-optimizer-get-enrollment-statuses-for-organization-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-statuses-for-organization-response-schema.json\",\n  \"title\": \"GetEnrollmentStatusesForOrganizationResponse\",\n  \"description\": \"GetEnrollmentStatusesForOrganizationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountEnrollmentStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountEnrollmentStatuses\"\n        },\n        {\n          \"description\": \"An array of objects that describe the enrollment statuses of organization member accounts.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of account\
  \ enrollment statuses.</p> <p>This value is null when there are no more pages of account enrollment statuses to return.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-enrollment-statuses-for-organization-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEnrollmentStatusesForOrganizationResponse
---
