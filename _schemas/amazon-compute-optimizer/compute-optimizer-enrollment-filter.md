---
description: Describes a filter that returns a more specific list of account enrollment statuses. Use this filter with the <a>GetEnrollmentStatusesForOrganization</a> action.
layout: schema
name: EnrollmentFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-enrollment-filter-schema.json
slug: compute-optimizer-enrollment-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-enrollment-filter-schema.json\",\n  \"title\": \"EnrollmentFilter\",\n  \"description\": \"Describes a filter that returns a more specific list of account enrollment statuses. Use this filter with the <a>GetEnrollmentStatusesForOrganization</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnrollmentFilterName\"\n        },\n        {\n          \"description\": \"<p>The name of the filter.</p> <p>Specify <code>Status</code> to return accounts with a specific enrollment status (for example, <code>Active</code>).</p>\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n\
  \          \"description\": \"<p>The value of the filter.</p> <p>The valid values are <code>Active</code>, <code>Inactive</code>, <code>Pending</code>, and <code>Failed</code>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-enrollment-filter-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: EnrollmentFilter
---
