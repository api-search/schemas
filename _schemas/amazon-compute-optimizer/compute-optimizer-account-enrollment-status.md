---
description: Describes the enrollment status of an organization's member accounts in Compute Optimizer.
layout: schema
name: AccountEnrollmentStatus
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: lastUpdatedTimestamp
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-account-enrollment-status-schema.json
slug: compute-optimizer-account-enrollment-status
source_filename: compute-optimizer-account-enrollment-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-account-enrollment-status-schema.json\",\n  \"title\": \"AccountEnrollmentStatus\",\n  \"description\": \"Describes the enrollment status of an organization's member accounts in Compute Optimizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The account enrollment status.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusReason\"\
  \n        },\n        {\n          \"description\": \"<p>The reason for the account enrollment status.</p> <p>For example, an account might show a status of <code>Pending</code> because member accounts of an organization require more time to be enrolled in the service.</p>\"\n        }\n      ]\n    },\n    \"lastUpdatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTimestamp\"\n        },\n        {\n          \"description\": \"The Unix epoch timestamp, in seconds, of when the account enrollment status was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-account-enrollment-status-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: AccountEnrollmentStatus
---
