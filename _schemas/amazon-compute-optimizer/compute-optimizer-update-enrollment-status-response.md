---
description: UpdateEnrollmentStatusResponse schema
layout: schema
name: UpdateEnrollmentStatusResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-update-enrollment-status-response-schema.json
slug: compute-optimizer-update-enrollment-status-response
source_filename: compute-optimizer-update-enrollment-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-update-enrollment-status-response-schema.json\",\n  \"title\": \"UpdateEnrollmentStatusResponse\",\n  \"description\": \"UpdateEnrollmentStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The enrollment status of the account.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusReason\"\n        },\n        {\n          \"description\": \"The reason for the enrollment status of the account. For example, an account might show a status of <code>Pending</code> because member accounts of an organization require more time to be\
  \ enrolled in the service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-update-enrollment-status-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: UpdateEnrollmentStatusResponse
---
